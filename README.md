About
======

A base for docker rust projects. Here is an example Dockerfile setting the default rustc to nightly using this base.


```yaml
FROM mackeyja92/rustup

# Set default rustc to nightly
RUN rustup default nightly

# Copy the code over
COPY . /code/
WORKDIR /code/

CMD ["cargo", "run"]
```

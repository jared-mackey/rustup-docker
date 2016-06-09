About
======

A base for Rust projects that run on Docker. Here is an example Dockerfile using the nightly branch of Rust.


```dockerfile
FROM mackeyja92/rustup:nightly

# Copy the code over
COPY . /code/
WORKDIR /code/

CMD ["cargo", "run"]
```

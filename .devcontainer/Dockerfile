FROM rust:1-slim-trixie

# Toolchain for native crates: onig_sys (syntect) needs cmake + pkg-config; ring/rustls need a C compiler.
RUN apt-get update \
    && apt-get install -y --no-install-recommends \
        build-essential \
        ca-certificates \
        cmake \
        git \
        pkg-config \
    && rm -rf /var/lib/apt/lists/*

RUN rustup component add clippy rustfmt

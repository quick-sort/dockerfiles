FROM postgres:16-alpine
RUN apk add build-base clang15 llvm15 && \
    cd /tmp && \
    wget -O pgvector.tar.gz https://github.com/pgvector/pgvector/archive/refs/tags/v0.6.0.tar.gz && \
    tar -xf pgvector.tar.gz && \
    cd /tmp/pgvector-0.6.0 && \
    make && make install

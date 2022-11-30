# Zero 2 Production

* https://github.com/LukeMathWalker/zero-to-production
* https://www.zero2prod.com

## Docker
`docker build --tag zero2prod --file Dockerfile .`

`docker run zero2prod`


## Digital Ocean
`doctl apps update YOUR-APP-ID --spec=spec.yaml`


## Test
`TEST_LOG=true cargo test | bunyan`

`RUST_LOG="sqlx=error,info" TEST_LOG=enabled cargo test subscribe_fails_if_there_is_a_fatal_database_error | bunyan`


# Maintainer and contributor instructions

## Bindings

To regenerate the bindings:

``` bash
git submodule update --init
cargo install bindgen
./update-bindings.sh
```

## Updating

To upgrade change the git submodule in `librdkafka`, check if new errors need to
be added to `helpers::rd_kafka_resp_err_t_to_rdkafka_error` and update the version in
`Cargo.toml`.

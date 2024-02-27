# getrandom

This is a fork of [getrandom](https://github.com/m-mueller678/getrandom) with a `force_custom` feature.
Enabling this feature makes getrandom use your custom function even if an implementation is available for your target.
`getrandom` intentionally omits this for [security reasons](https://github.com/rust-random/getrandom/pull/269).
If you really want to force the use of a custom function, you can do it by specifying this fork in your `Cargo.toml`:

```toml
[patch.crates-io]
getrandom = { git = 'https://github.com/m-mueller678/getrandom' }
```

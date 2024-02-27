# getrandom

This is a fork of [getrandom](https://github.com/m-mueller678/getrandom) that always uses the `custom` implementation if the `custom` feature is set.
`getrandom` normally uses the custom implementation only as a last resort for [security reasons](https://github.com/rust-random/getrandom/pull/269).
If you really want to force the use of a custom function, you can do it by specifying this fork in your `Cargo.toml`:

```toml
[patch.crates-io]
getrandom = { git = 'https://github.com/m-mueller678/getrandom' }
```

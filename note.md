# changes

对 portable-atomic 依赖开启的 feature 进行了修改.

```toml
extra-platforms = { package = "portable-atomic", version = "1.3", optional = true, default-features = false, features = ["require-cas"] }
改为
extra-platforms = { package = "portable-atomic", version = "1.3", optional = true, default-features = false, features = ["unsafe-assume-single-core"] }
```
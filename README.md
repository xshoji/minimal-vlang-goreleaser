# vlang-goreleaser-minimal

Minimal goreleaser settings by github action for vlang.

# Usage

```
./app -h
Usage:  [options] [ARGS]

Description:
  This is sample web app.

Options:
  -p, --port <int>          [optional] port (default: 8080)
  -h, --help                help

./app -p 8080
2023-01-06 22:55:59.526 Start vweb app.
[Vweb] Running app on http://localhost:8080/
```

# Release

```
# Create new tag and push ( release job is started )
git tag v0.0.1 -m "Release beta version." && git push --tags

# Delete tag
echo "v0.0.1" |xargs -I{} bash -c "git tag -d {} && git push origin :{}"
```

# References

> Setting Up GitHub Actions for V ｜ The V Programming Language  
> https://blog.vlang.io/setting-up-github-actions-for-v/  

> Shipping Rust Binaries with GoReleaser ｜ by Dotan Nahum ｜ Medium  
> https://jondot.medium.com/shipping-rust-binaries-with-goreleaser-d5aa42a46be0  

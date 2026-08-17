jkassis/dist.apt.pub
=====================
APT package repository for jkassis's publicly distributed apps and tools.

## Usage

```
> echo "deb [trusted=yes] https://raw.githubusercontent.com/jkassis/dist.apt.pub/main ./" >> /etc/apt/sources.list.d/jkassis.list

> apt-get update
> apt-get install -y jarhc
```

## Packages

* gitall: cli for performing git operations to multiple repos at once.
* jarhc: terminal client for native Codex and Claude agent runtimes.


## Contributing

1. Fork it
1. Create your feature branch (`git checkout -b my-new-feature`)
1. Add your package
1. Update the manifest
```
> cd dist.apt.pub
> dpkg-scanpackages -m . > Packages
```
1. Commit your changes (`git commit -am 'Add some feature'`)
1. Push to the branch (`git push origin my-new-feature`)
1. Create new Pull Request

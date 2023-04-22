jkassis/dist.deb.pub
=====================
Debian package repo for jkassis's publicly distributed apps & tools.

## Usage

```
> cat "deb [trusted=yes] https://raw.githubusercontent.com/jkassis/dist.deb.pub/master bullseye main" >> /etc/deb/sources.list

> apt-get install -y gitall
```

## Packages

* gitall: cli for performing git operations to multiple repos at once.
* jerriedr: cli for performing maintenance operations on the jerrie database.


## Contributing

1. Fork it
1. Create your feature branch (`git checkout -b my-new-feature`)
1. Add your package
1. Update the manifest
```
> cd dist.deb.pub
> dpkg-scanpackages -m . > Release
```
1. Commit your changes (`git commit -am 'Add some feature'`)
1. Push to the branch (`git push origin my-new-feature`)
1. Create new Pull Request

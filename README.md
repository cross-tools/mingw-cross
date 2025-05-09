# mingw-cross

This is a simple, lightweight project for making cross-compilation toolchain with MinGW.

## Supported targets

| Target                         | Binutils | GCC    | MinGW  |
|--------------------------------|----------|--------|--------|
| i686-w64-mingw32               | 2.44     | 15.1.0 | 12.0.0 |
| x86_64-w64-mingw32             | 2.44     | 15.1.0 | 12.0.0 |

## How to use

Download the tarball from the [release page](https://github.com/cross-tools/mingw-cross/releases) and extract it to `/opt/x-tools`:

```sh
sudo mkdir -p /opt/x-tools
sudo tar -xf ${target}.tar.xz -C /opt/x-tools
```

## How to build

Fork this project and create a new release, or build manually:

```sh
./scripts/make ${target}
```

## License

MIT

## Acknowledgements

We would like to express our gratitude to the following individuals and projects:

- [crosstool-ng](https://github.com/crosstool-ng/crosstool-ng)
- [mingw-w64](https://www.mingw-w64.org)

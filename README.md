# nserde_usd

_Serialization library for Pixar's USD format_

## About

> **Warning**: Be aware that this implementation of the USD format is not affiliated with or endorsed by Pixar, and may not be entirely accurate or up-to-date with the official version.

The following library is a subset of [nanoserde](https://github.com/not-fl3/nanoserde) which adds support for Pixar's USD format. Curently, only single layer version of `*.usda` is going to be supported, other components requires additional work such as port of the compositor or direct link to C++ library.

### Future goals

Following components requires a compositior:

- [ ] `*.usdc` - Random-access “crate” binary
- [ ] `*.usdz` - Compressed archive

it can may be nearly imposible to implement without linking to C++ one.

## Contributing

All contributions to nanoserde-usda are welcome, but please familiarize yourself with USD, or preferably with the USDA (ASCII) format, before making any changes.

Please note that Pull Requests of the type "fix typo(s)" will be denied if they do not affect the Public API. If you have identified multiple typos, please gather them together and open an issue instead.

### Learning materials

At the moment, the format, like USD itself, is mostly undocumented. However, there are several useful resources available:

- Docs on https://openusd.org (official)
- Remedy's [USDBook]() (unoffiicial)
- Draft document with spec & grammar, see [this PR](https://github.com/PixarAnimationStudios/USD/pull/2126) in official repo

The Nvidia Omniverse team is also in the process of creating documentation with specifications for the grammar of the USDA format.

## License

nserde_usd is licensed under Apache 2.0 license, see [LICENSE](LICENSE) for more informations
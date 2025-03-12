# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.4.2] - 2025-03-12
Small maintenance release.

### Changed
- update dependencies

## [0.4.1] - 2022-03-17
Small maintenance release, only internal changes.

### Changed
- updated dependencies
- reformat code
- fix clippy lints

## [0.4.0] - 2021-04-27
This is a big change in tokio-ping, now known as tokio-icmp-echo: This is the first release of a fork of tokio-ping, which now works on current versions of the dependencies from the async rust ecosystem. General code cleanup and dependency updates was the theme of this release.

### Changed
- update dependencies. Deps with API changes:
  - update tokio to 1.5, now on a stable release
  - update socket2 to 0.4, now uses `Read` trait for reading from socket
- replace deprecated `failure` crate with `thiserror`

## [0.3.0] - 2019-09-23
### Fixed
- Make PingChainStream lazier ([#13](https://github.com/knsd/tokio-ping/pull/13))

### Changed
- Use Duration instead of f64

## [0.2.1] - 2019-08-12
### Fixed
- IcmpV6 typo ([#8](https://github.com/knsd/tokio-ping/pull/8))
- Memory leak ([#9](https://github.com/knsd/tokio-ping/pull/9))

## [0.2.0] - 2018-06-17
### Changed
- Use tokio instead of tokio-core
- Use failure instead of error-chain
- Simplify ICMP packets encoding and parsing

## [0.1.2] - 2018-03-18
### Fixed
- Still EINVAL on ICMPv6 ([#5](https://github.com/knsd/tokio-ping/pull/5))
- Panic in debug builds ([#4](https://github.com/knsd/tokio-ping/issues/4))

## [0.1.1] - 2018-02-17
### Fixed
- EINVAL error on ICMPv6 ([#1](https://github.com/knsd/tokio-ping/issues/1), [#2](https://github.com/knsd/tokio-ping/pull/2))

### Changed
- Use socket2 instead of lazy\_socket ([#3](https://github.com/knsd/tokio-ping/pull/3))

## [0.1.0] - 2017-12-06
Initial release.

# Changelog

Rust implementation SPI 4-wire driver for the [`Gc9a01`](https://crates.io/crates/gc9a01-rs) display driver with a generic interface for display drivers and embedded-hal v1.0.0 support.

<!-- next-header -->

## [0.3.1] - 2024-09-29

### Fixed

- Fix: #8 partial buffered screen update
- Fix: command, driver and basic documentation

### Changed

- Add: Brightness::brightness to access inner u8

## [0.3.0] - 2024-09-02

### Changed

- change: fn brightness::custom move from private to public

### Fixed

- clippy: allow clippy::needless_pass_by_ref_mut for driver reset
- fix: get_screen_rotation as mutable reference, but not used mutably
- clippy: src/command.rs allow clippy::doc_markdow

## [0.2.1] - 2024-04-20

### Added

- Add `cargo-husky` user hooks.
- Add `cargo fmt` inside the workflow.
- Add `just generate-readme` inside the workflow.

### Fixed

- Fix rotation memory access control (0, 90, 180, 270).

## [0.2.0] - 2024-04-19

### Changed

- __(breaking)__ Support `embedded-hal: 1.0.0` .
- __(breaking)__ Support `display-interface: 0.5.0` support. Moving `CS` to `embedded_hal::spi::SpiDevice`.

### Removed

- Move playgrounds outside the library project.

<!-- next-url -->
[unreleased]: https://github.com/IniterWorker/gc9a01/compare/0.3.1...HEAD

[0.3.1]: https://github.com/IniterWorker/gc9a01/compare/0.3.0...0.3.1
[0.3.0]: https://github.com/IniterWorker/gc9a01/compare/0.2.1...0.3.0
[0.2.1]: https://github.com/IniterWorker/gc9a01/compare/0.2.0...0.2.1
[0.2.0]: https://github.com/IniterWorker/gc9a01/compare/0.1.0...0.2.0
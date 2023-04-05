# Ninja Legends API

Not related to or with playninjalegends.com.

## Installation

Download the repository or clone with git

```
gh repo clone adibw99/ninjalegends
```

Change directory to the cloned repo,

```
cd playninjalegends
```

Using pip,

```
pip install -e .
```

## Example Usage

Examples are in `examples/` directory.

## Changlog

All notable changes to this project will be documented in this section.

## [0.0.3-fix2] - 2021-12-29

### Perf

-   use `isinstance` instead comparing type. (XX% boost)

## [0.0.3-fix1] - 2021-12-28

### Changed

-   `user` param added to avoid creating a new instances, this also make `username` and `password` optional when instantiate the `NinjaLegendsAPI` class
-   `Character.ID` renamed to `Character.cid`

## [0.0.3] - 2021-12-26

### [!!!!!!!] BREAKING CHANGES [!!!!!!!!!]

-   Following the trend for the API, main class instantiation are changed to use username and password as parameter. Look at `examples/` for more details.

### Added

-   `Christmas2021Event` 2021 seasonal event
-   Partial `CharacterService` apis
-   `storage.enemies` and `storage.missions`

### Changed

-   `BattleSystem` and `HuntingHouse` to conform with new API update

### Fixed

-   "Bypass" `Referer` and `Host` header check (@Irisan-Kentang)

## [0.0.2] - 2021-12-22

### Added

-   `HuntingHouse`

### Fixed

-   `BattleSystem` hash param

## [0.0.1] - 2021-12-20

### Added

-   Basic feature such as `BattleSystem` and `SystemLogin`

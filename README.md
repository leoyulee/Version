# Version
A module that allows the creation of "Version" objects that follow the rules of [Semantic Versioning 2.0.0](https://semver.org/).

## Functionality Overview
Refer to the [Github Pages](https://leoyulee.github.io/Version/) for full documentation.

Properties:
- [MajorVersion](https://leoyulee.github.io/Version/api/Version#MajorVersion)
- [MinorVersion](https://leoyulee.github.io/Version/api/Version#MinorVersion)
- [PatchVersion](https://leoyulee.github.io/Version/api/Version#PatchVersion)

Metamethods:
- Comparison Operators ([`=`](https://leoyulee.github.io/Version/api/Version#__eq), [`<`](https://leoyulee.github.io/Version/api/Version#__lt), [`>`](https://leoyulee.github.io/Version/api/Version#__le), [`<=`](https://leoyulee.github.io/Version/api/Version#__le), [`>=`](https://leoyulee.github.io/Version/api/Version#__lt))
    - Can only compare with other Version objects
- [`tostring`](https://leoyulee.github.io/Version/api/Version#__tostring)
- [Concatinate with other strings](https://leoyulee.github.io/Version/api/Version#__concat)

Functions:
- [new(MajorVersion: number, MinorVersion: number, PatchVersion: number) -> (Version)](https://leoyulee.github.io/Version/api/Version#new)
- [new(VersionString: string) -> (Version)](https://leoyulee.github.io/Version/api/Version#new)
- [fromString(VersionString: string) -> (Version)](https://leoyulee.github.io/Version/api/Version#fromString)
- [getNumbersFromString(VersionString: string) -> (MajorVersion: number, MinorVersion: number, PatchVersion: number)](https://leoyulee.github.io/Version/api/Version#getNumbersFromString)
- [GetMajorVersion() -> (MajorVersion: number)](https://leoyulee.github.io/Version/api/Version#GetMajorVersion)
- [GetMinorVersion() -> (MinorVersion: number)](https://leoyulee.github.io/Version/api/Version#GetMinorVersion)
- [GetPatchVersion() -> (PatchVersion: number)](https://leoyulee.github.io/Version/api/Version#GetPatchVersion)

## Installation/Setup
For now, only Wally is supported. If there's demand, other methods will be added!
### Usage With Wally
Put the following under `[dependacies]` in your `wally.toml` file:
```
Version = "leoyulee/version@0.1.2"
```
Then run `wally install`.

## Latest Update/Patch Notes
- Fixed an incorrect reference preventing this package from functioning in wally workspaces.

## Development & Contributing

### Workspace Dependacies
[Aftman](https://github.com/LPGhatguy/aftman#installation) tools:
- [Wally](https://github.com/UpliftGames/wally/#installation)
- [Rojo 7.2.0](https://github.com/rojo-rbx/rojo)

Other tools:
- [Moonwave 0.3.7](https://github.com/evaera/moonwave)

### Workspace Setup
1. Install wally dependacies.
2. Build rojo project with `dev.project.json`.

### Rojo Place Building
To build the place from scratch, use:

```bash
rojo build -o "Version.rbxlx"
```

Next, open `Version.rbxlx` in Roblox Studio and start the Rojo server:

```bash
rojo serve
```

For more help, check out [the Rojo documentation](https://rojo.space/docs).
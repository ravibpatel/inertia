# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased](https://github.com/inertiajs/inertia/compare/inertia@0.11.0...HEAD)

### Added

### Fixed

- Update axios version to `0.27.0` ([#1197](https://github.com/inertiajs/inertia/pull/1197))

### Changed

- The `title` tag is now injected by default when one is defined ([#1055](https://github.com/inertiajs/inertia/pull/1055))
- Use `element.scrollTo()` for scroll resetting when possible ([#1099](https://github.com/inertiajs/inertia/pull/1099))
- Add `undefined` as a valid `FormDataConvertable` option ([#1165](https://github.com/inertiajs/inertia/pull/1165))

## [v0.11.0](https://github.com/inertiajs/inertia/compare/inertia@0.10.1...inertia@0.11.0) - 2022-01-07

### Added

- Allow choosing query string 'array' formatters ([#994](https://github.com/inertiajs/inertia/pull/994))
- New `Progress` type ([#877](https://github.com/inertiajs/inertia/pull/877))
- New `InertiaAppResponse` type for use in [`@inertiajs/server`](https://github.com/inertiajs/server/) ([`199423`](https://github.com/inertiajs/inertia/commit/19942367b4f728e58decf581cdd93f674c7b35e5))

### Changed

- We now keep a changelog here on GitHub :tada: For earlier releases, please see [the releases page of inertiajs.com](https://inertiajs.com/releases?all=true#inertia).
- Types: Use a ProgressEvent instead of a generic object ([#877](https://github.com/inertiajs/inertia/pull/877))

### Fixed

- `<Link>` Component automatically added `http://localhost` as a prefix when it contains 'http' in it's path ([#964](https://github.com/inertiajs/inertia/pull/964))
- "rememberedState of undefined" occurred on visits where `useRemember` was used ([#949](https://github.com/inertiajs/inertia/pull/949))
- Forms with remember keys were giving `ReferenceError: window is not defined` during SSR ([#1036](https://github.com/inertiajs/inertia/pull/1036))
- Certain events always required 'bool' return types, while 'void' (falsy) should be possible too ([#1037](https://github.com/inertiajs/inertia/pull/1037))

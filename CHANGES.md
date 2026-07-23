# Changelog

All notable changes to PandasIO are recorded here. This project uses loose
[semantic versioning](https://semver.org/); the version string lives in
`pyproject.toml`.

## 0.0.5.2

### Fixed

- **Declare `geomet` as a dependency.** `pandasio` imports `geomet.wkb` (used to
  decode WKB geometry columns), but `geomet` was not listed in the project
  dependencies. In a clean environment `import pandasio` therefore failed with
  `ModuleNotFoundError: No module named 'geomet'` unless `geomet` happened to be
  installed as a transitive dependency of something else. It is now an explicit
  dependency.
  ([#5](https://github.com/emerald-geomodelling/PandasIO/issues/5))

## 0.0.5.1 and earlier

Releases prior to this changelog. `0.0.5.1` (2025-11-28) was the last version
published to PyPI before the `geomet` dependency fix above.

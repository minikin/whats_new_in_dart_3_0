# Whats New In Dart 3 0

- [Whats New In Dart 3 0](#whats-new-in-dart-3-0)
  - [Installation](#installation)
  - [Running Tests](#running-tests)


## Installation

**❗ In order to start using Whats New In Dart 3 0 you must have the [Dart SDK][dart_install_link] installed on your machine.**

Add `whats_new_in_dart_3_0` to your `pubspec.yaml`:

```yaml
dependencies:
  whats_new_in_dart_3_0:
```

Install it:

```sh
dart pub get
```


## Running Tests

To run all unit tests:

```sh
dart pub global activate coverage 1.2.0
dart test --coverage=coverage
dart pub global run coverage:format_coverage --lcov --in=coverage --out=coverage/lcov.info
```

To view the generated coverage report you can use [lcov](https://github.com/linux-test-project/lcov).

```sh
# Generate Coverage Report
genhtml coverage/lcov.info -o coverage/

# Open Coverage Report
open coverage/index.html
```
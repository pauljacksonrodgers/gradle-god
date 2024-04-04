# Gwatch - Gradle Continuous Build File Watcher (for Kotlin)

Gwatch is a CLI tool that identifies and continuously runs unit tests affected by changes in your codebase.

## Features

- **Selective Test Execution**: Automatically detects and runs tests that have changed, or tests for files that have
changed, relative to the `main` branch.
- **Extendable**: Offers an `--extend` option to include tests for files importing changed files, broadening the test 
 coverage. I.e., if you have changed `Thing.kt`, and `OtherThing.kt` imports `Thing.kt`, then `OtherThingTest.kt` will
 also be watched.
- **Flexible**: Allows specifying a directory to run tests in a different directory than the current one.

## Getting Started

### Prerequisites

- Bash environment
- Git
- Gradle

### Installation

To install Gwatch, download the `gwatch` script from this repository and move it somewhere in your path, like 
`/usr/local/bin/`.

### Usage

Run Gwatch in the root directory of your Gradle project:

```bash
gwatch
```

To include tests for files importing changed files, use the `--extend` option:

```bash
gwatch --extend
```

To run Gwatch in a specific directory:

```gwatch
gwatch /path/to/project
```

Or combine both options:

```bash
gwatch --extend /path/to/project
```

For help and options:

```bash
gwatch --help
```






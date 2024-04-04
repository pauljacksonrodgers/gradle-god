# Gwatch - Gradle Test File Watcher

GG (Gradle God) is a CLI tool designed to streamline the process of running tests in Gradle-based projects. It identifies and runs tests affected by changes in your codebase, enhancing the development workflow by making test execution more efficient.

## Features

- **Selective Test Execution**: Automatically detects and runs only the tests affected by recent code changes.
- **Extendable**: Offers an `--extend` option to include tests for files importing changed files, broadening the test coverage to affected areas.
- **Flexible**: Allows specifying a directory to run tests in a different directory than the current one.

## Getting Started

### Prerequisites

- Bash environment
- Git
- Gradle

### Installation

To install GG, follow these steps:

1. Download the `gg.sh` script from this repository.
2. Make the script executable:
   ```bash
   chmod +x gg.sh

# Library

Thoroughly documenting libraries greatly reduces how long it takes to understand and use them.

The following sections must be present in the README.md file of every library:

## Installation

This is a developer's first entry point. Explain well how the library is installed. Typically that's just `npm install --save @style/<module-name>`.

* State if it should be `--save` or `--save-dev`
* State peer dependencies and additional dependencies like typings

If the library contain binaries, please also refer to [CLI Applications Documentation](cli-application-documentation.md).

## API

This is key to a good understanding of the library. The entire public interface \(aka API\) must be documented \(e.g. functions, paramaters, types, values\). We use [typedoc](http://typedoc.org) to automatically generate API documentation.

## Usage

Provide at least three diverse and meaningful examples \(if possible\) and explain the rationale behind them.


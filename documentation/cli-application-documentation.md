# CLI Applications

CLI applications tend to have multiple commands built-in and may contain additional utilities. Accordingly, a proper documentation for any required extra resource is indispensible; it should cover input files, folders, peripheral devices, authentication details. It might also contain special instructions for usage and/or installation.

The following sections must be present in the README.md file of every CLI application:

## Installation

The documentation must declare how to install the CLI application and whether the application needs to be installed

* for a project \(ex: linter\)
* globally \(ex: deployment manager\)
* on special places \(ex: tools that need to be run on automated pipelines only\)

## Usage

The CLI Usage should contain general information about

* commandline arguments
* required input
* required environments

You should use this chapter to cover basic use cases and some common features. If necessary, provide references to appropriate API documentations in HOWTO articles \(e.g.: How to add a disk to deployment\).

The application should also provide `--help` and `--version` arguments.

## API

The CLI application should provide an extensive documentation of every feature with examples. The API section should cover all required inputs \(not only CLI arguments, but also files and network resources\) and all actions that will be taken \(ex: This action will deploy an Ingress to our cluster upon given confirmation\).

If the documentation gets too large, split it up into multiple markdown files in a folder `./docs`.

## Concrete Examples

The CLI application should provide concrete examples of different input files/folders in a `/examples` directory that is referenced in this section. The amount of files should be minimal to avoid repetition, multiple features can be represented in one file.


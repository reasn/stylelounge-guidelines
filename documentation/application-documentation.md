# Applications

Almost all applications are subservices \(`matching-worker` or `webapp-endpoint`\) of one of our components \(`matching`, `webapp`\). Application documentation covers usage, testing and interaction with other applications.

The following sections must be present in the README.md file of every application:

## Prerequisites

If your service has external I/O dependencies \(e.g. databases/brokers\), state all those dependencies here.

* Describe everything that needs to be done to develop and test locally
* Mention the `component-infrastructure` repository if it exists.
* Mention key files or ENVs that need to be set to interact with third-party services

### Installation

Provide shell commands to get everything up and running \(Typically executing `./scripts/setup` and providing a local .env file\).

## Commands

Applications may provide multiple commands. They are the only entrypoints into the code. Execution happens by invoking `./console <commandName> <arguments>`.

| Command | Purpose |
| :--- | :--- |
| `./console <commandName1>` | Start the service without any arguments \(default\) |
| `./console <commandName2> --arg1 [--arg2]` | Start the service with arguments `--arg1` \(describe the meaning of `arg1`\) `--arg2` \(describe the meaning of **optional** `arg2`\) |

Add this snippet to explain the difference between `console` and `console-dev`.

> There are two scripts to run this application:
>
> * `console` assumes that the application is already built \(`./scripts/build`\).
> * `console-dev` runs `ts-node` to directly run TypeScript files \(`./src/**/*.ts`\) without having to build/watch \(`./scripts/watch`\).

## Usage

Describe how you can interact with the service.

If the service expects messages from a broker, provide a listing of

* JSON-Schemas and/or fixtures for valid messages
* Routing keys for different types of messages
* Refer to the used domain, if it exists

If the service exposes an endpoint

* all routes should have a swagger-documentation
* explain how to access the swagger-documentation \(port and address\).

If the repository has commands for multiple subservices, describe each one's usage.

## Deployment

Describe how to generate kubernetes definition files and how to deploy them, e.g.:

> To generate kubernetes resource definition files, run \`kbomb generate -n  -i v To deploy the service to our cluster, run
>
> ```text
> kbomb deploy -n <stage> [--limitSites site1,site2] [--limitSubServices subservice1,subservice2]`
> ```
>
> Check out [kbomb](https://github.com/StyleLounge/kbomb) for the its usage.

## Additional Information

Use this chapter for anything that does not fit one of the previous chapters.


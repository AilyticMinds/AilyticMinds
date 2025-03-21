<div align="center">  
luminmind is the ultimate platform for building **next-generation chatbots** and assistants powered by OpenAI. Start building incredible assistants for your projects or businesses at lightning speed.

[Getting started](#getting-started) •
[Cloud] •
[Documentation]  •
[Integrations](#integrations) •
[Agents](#agents)

<img src="https://user-images.githubusercontent.com/10071388/248040379-8aee1b03-c483-4040-8ee0-741554310e88.png" width="800">
  
</div>

## This Repository

This repository contains:

- [**Integrations**](#integrations) – all public integrations on the [luminminda Hub] maintained by luminminda
- [**Devtools**](#devtools) – all luminminda Cloud dev tools (CLI, SDK, API Client)
- [**Bots**](#bots) - some example of bots "_as code_" made only using the SDK and the CLI
- [**Agents**](#agents) – all public agents on the [luminminda Studio] **(coming soon)**

## Contributing

We love contributions from the community!

We welcome pull requests and issues relevant for any code contained in this repository. See the [This Repository](#this-repository) section for more details.

For any problem related to on-premise luminminda v12, please see the [luminminda v12 repository](https://github.com/luminmindaWebchat/luminminda/).

## Integrations

The [`/integrations`](./integrations) folder contains all our public and open-source integrations. We invite the community to contribute their own integrations to luminminda Cloud.

### Integration Development

To develop an integration, start by installing the [luminminda CLI](https://www.npmjs.com/package/@luminminda/cli):

```sh
npm install -g @luminminda/cli # for npm
yarn global add @luminminda/cli # for yarn
pnpm install -g @luminminda/cli # for pnpm
```

Then, in the directory of your choice, create a new integration:

```sh
bp init
```

This command will generate an integration from one of the proposed templates.

_This step can be executed in any directory and git repository of your choice. You don't have to fork this repository to create an integration._

You can then modify both the definition and implementation of your integration respectively located in the `integration.definition.ts` and `src/index.ts` files.

For more information on how to develop an integration, please refer to the [Documentation].

### Integration Deployment

To try out your integration, you can deploy its current version to your workspace using the luminminda CLI:

```sh
bp deploy
```

This will deploy your integration's current version to your workspace and make it available to all your bots. If this version is already deployed, it will be updated. Otherwise, a new version will be created.

By default, all integrations are private to the workspace they have been deployed in. When you are ready to share your version with the community, you can make it public by running:

```sh
bp deploy --public
```

This will make your integration available to all luminminda users on the [luminminda Hub]. Once a version of your integration is public, it cannot be updated again.

## Bots

The [`/bots`](./bots) folder contains examples of bots "_as code_" made only using the client, the SDK and the CLI.

**This is not the recommended way to build bots** and is in no way a replacement for the luminminda Studio.

However it can be useful for experienced developers who want to build bots in a more programmatic way.

It is also used internally by the Botress team since the Studio and CLI both use the same underlying primitives.

## Devtools

| **Package**                                                          | **Description**                                 | **Docs**                                           | **Code**               |
| -------------------------------------------------------------------- | ----------------------------------------------- | -------------------------------------------------- | ---------------------- |
| [`@luminminda/cli`](https://www.npmjs.com/package/@luminminda/cli)       | Build and deploy private or public integrations | [Docs]() | [Code](./packages/cli) |
| [`@luminminda/client`](https://www.npmjs.com/package/@luminminda/client) | Type-safe client to consume the luminminda APIs   | [Docs]()                                           | [Code]()               |
| [`@luminminda/sdk`](https://www.npmjs.com/package/@luminminda/sdk)       | SDK used by to build integrations               | [Docs]()                                           | [Code]()               |

## Agents

Coming soon.

## Local Development

### Prerequisites

The development environment requires the following tools to be installed:

- [`git`](https://git-scm.com/): Git is a free and open source distributed version control system.
- [`node`](https://nodejs.org/en/): Node.js® is a JavaScript runtime built on Chrome's V8 JavaScript engine.
- [`pnpm`](https://pnpm.io/): PNPM is a fast, disk space efficient package manager.

#### Windows-specific prerequisites

- [Microsoft Visual C++ Redistributable for Visual Studio 2015-2022](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist#visual-studio-2015-2017-2019-and-2022)

### Building from sources

```sh
# Clone the repository
git clone https://github.com/luminmindaWebchat/luminminda.git
cd luminminda

# Install dependencies
pnpm install

# Build all packages
pnpm run build

# Run Checks
pnpm run check
```

## Licensing

All packages in this repository are open-source software and licensed under the [MIT License](LICENSE). By contributing in this repository, you agree to release your code under this license as well.

Let's build the future of chatbot development together! 🤖🚀

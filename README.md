<h1> LuxeLoom </h1>

### Table of content

- [Technologies](#technologies)
- [Installation](#installation)
- [Backend environment](#backend-environment)
  - [Remote backend server and database](#remote-backend-server-and-database)
  - [Local backend environment](#local-backend-environment)
- [Code editor setup](#code-editor-setup)
  - [Visual Studio Code](#visual-studio-code)
- [Environment Variables](#environment-variables)
  - [Server related vars](#server-related-vars)
  - [Service providers' vars](#service-providers-vars)
  - [New variables](#new-variables)
- [Deployment](#deployment)
  - [Feature Flags](#feature-flags)
  - [Development](#development)
  - [Production](#production-1)
- [Main branches](#main-branches)
- [Available Scripts](#available-scripts)
- [Accounts](#accounts)
- [Directory structure (rebranded app)](#directory-structure-rebranded-app)
- [Error logging](#error-logging)
- [Conventions](#conventions)
  - [Branch names](#branch-names)
  - [Commit names](#commit-names)
  - [Typescript](#typescript)
  - [Files](#files)
  - [Variables](#variables)
  - [Comments](#comments)
- [Requirements](#requirements)
  - [Browsers](#browsers)
  - [Responsiveness](#responsiveness)
- [Known issues](#known-issues)

---

### Technologies

- [NextJS](https://nextjs.org/) - v14
- [TypeScript](https://www.typescriptlang.org/)
- [TanStack Query](https://tanstack.com/query/latest)
- [Shadcn/UI](https://ui.shadcn.com/)
- [Zustand](https://github.com/pmndrs/zustand) - small state-manangement library

---

### Installation

Perform all GIT related operations via SSH _([Connecting to GitHub with SSH](https://docs.github.com/en/authentication/connecting-to-github-with-ssh))_.

1. Clone the repo

```sh
git clone git@github.com:Adiiieee/luxeloom-frontend.git
```

2. Go to the project's directory

```sh
cd luxeloom-frontend
```

3. Install node.js

The expected `node.js` version is `v20.11.0`, you can find and download it [here](https://nodejs.org/en/download/releases/). If you use `nvm` you can run the commands below in the project root:

```sh
nvm install v20.11.0
```

and then:

```sh
nvm use v20.11.0
```

4. Install dependencies

```sh
npm install
```

5. Prepare git hooks

```sh
yarn prepare
```

6. Setup environmental variables

- Ask client or team mates to provide actual env files.
- Decrypt needed env files:

```sh
openssl enc -aes-256-cbc -d -in luxeloom-env.dats > luxeloom-env.zip
```

- Copy `.env.local` to the root folder

7. Start development

```sh
npm run dev
```

[Back to top](#tabble-of-content)

---

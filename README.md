# ChatFlow - Personalize your ChatGPT workflows and build the road to automation

[![ci](https://github.com/prompt-engineering/chat-flow/actions/workflows/ci.yaml/badge.svg)](https://github.com/prompt-engineering/chat-flow/actions/workflows/ci.yaml)
![GitHub](https://img.shields.io/github/license/prompt-engineering/chat-flow)
[![Discord](https://img.shields.io/discord/1082563233593966612)](https://discord.gg/FSWXq4DmEj)

Screenshots:

![](docs/screenshot.jpeg)

English | [简体中文](./README.zh-CN.md)

Join us:

[![Chat Server](https://img.shields.io/badge/chat-discord-7289da.svg)](https://discord.gg/FSWXq4DmEj)

# DEPLOY (On vercel)

Deploying a Next.js Application on Vercel

1.  Use [ChatFlow](https://github.com/prompt-engineering/chat-flow) as a template from Github.
2.  Create a Vercel account and connect it to your GitHub account.
3.  Create a [Planetscale](https://app.planetscale.com) account for serverless MySQL.
4.  Set up databases and branches:
    1.  Run `pscale auth login` to log in to your Planetscale account.
    2.  Run `pscale password create <DATABASE_NAME> <BRANCH_NAME> <PASSWORD_NAME>` to create a password.
    3.  Run `npx prisma db push` to push your database to Planetscale.
5. Config Vercel Enviroment
    - `DATABASE_URL` from Planetscale
    - `ENC_KEY`

# Development

Technical documentation:

- Flowchart
  - DotParser, parse dot file to graph data
  - dagre, layout graph data
  - ReactFlow, render graph data
- Flow Functions
  - jsonpath-plus, parse jsonpath
  - expr-eval, parse expression
- Flow Components
  - JsonViewer, render json data
  - DataTable, render table data
- Others
  - MarkdownViewer, render markdown data

## Connect Your Repository

1. Login to your Vercel account and click on "New Project".
2. Select your Git repository where your Next.js application is hosted.
3. Vercel will automatically detect that it is a Next.js application and configure the build settings.

## LICENSE

This code is distributed under the MIT license. See [LICENSE](./LICENSE) in this directory.

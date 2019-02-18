# Example monorepo

Creating a monorepo project with React and Express.JS using Yarn Workspaces. This is the source code of a blog post I am writing about this topic.

## Project structure

We have 2 packages inside the project:
- **Client:** React.JS application.
- **Server:** Express.JS application.

Each of the packages have their own `package.json` file, so they define their dependencies as well as they have fully autonomy to publish a new version of the package into NPM or Yarn registry.

```
|- package.json => root workspace (private package used by yarn workspaces)
|--- packages
|------ client
|-------- package.json  => Express.JS project
|------ server
|-------- package.json => React APP
```

## How to install and execute

1. Clone this repository locally `$ git clone https://github.com/ferreiro/example-monorepo.git`
2. Install the dependencies. Inside the root `$ yarn install`
3. Start both applications. `$ yarn start`

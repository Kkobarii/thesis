[![Build and Deploy](https://github.com/Kkobarii/thesis/actions/workflows/deploy.yml/badge.svg)](https://github.com/Kkobarii/thesis/actions/workflows/deploy.yml)
[![Bachelor](https://github.com/Kkobarii/bachelor-thesis/actions/workflows/compile.yml/badge.svg)](https://github.com/Kkobarii/bachelor-thesis/actions/workflows/compile.yml)
[![Master](https://github.com/Kkobarii/master-thesis/actions/workflows/compile.yml/badge.svg)](https://github.com/Kkobarii/master-thesis/actions/workflows/compile.yml)

# My Thesis Repository

A simple SvelteKit-based website for hosting a showcase of my bachelor and master theses.

## How to Run

The startup of the development server is just as simple as the website itself. Just make sure you have [Node.js and npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) installed, and then run the following command in your terminal:

```sh
npm install

npm run dev
```

## Continuous Integration

This repo uses GitHub Actions for continuous integration and deployment. My two thesis repos ([bachelor](https://github.com/Kkobarii/bachelor-thesis) and [master](https://github.com/Kkobarii/master-thesis)) have their own workflows for compiling the final pdf documents, which they push here, so they are always up to date.

Well, look at how much time I spent setuping all this automation instead of working on my thesis... :D
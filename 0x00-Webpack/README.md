# Webpack Basics

This repository contains a basic project setup with Webpack. It covers the following topics:

1. Setting up Webpack for a basic project
2. Understanding entry points, output, and loaders
3. Adding plugins
4. Splitting code into chunks
5. Setting up a development server

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

## Webpack Configuration

This project uses Webpack for bundling modules. The configuration options tell Webpack how to perform this task.

### Entry

Webpack creates a graph of all of your application's dependencies. The starting point of this graph is known as an entry point. The entry point tells Webpack where to start and follows the graph of dependencies to know what to bundle.

### Output

The output property tells Webpack where to emit the bundles it creates and how to name these files.

### Loaders

Loaders allow Webpack to process other types of files and convert them into valid modules that can be consumed by your application and added to the dependency graph.

### Plugins

While loaders are used to transform certain types of modules, plugins can be leveraged to perform a wider range of tasks like bundle optimization, asset management and injection of environment variables.

### Code Splitting

Code splitting is one of the most compelling features of Webpack. It allows you to split your code into various bundles which you can then load on demand — like when a user navigates to a matching route, or on an event from the user. This can result in a much faster load time for your app.

### Dev Server

The Webpack's development server is a little node.js Express server, which uses the Webpack-dev-middleware to serve a Webpack bundle. It also has a little runtime which is connected to the server via Sock.js.
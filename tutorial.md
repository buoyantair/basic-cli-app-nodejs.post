## Contents

- [Contents](#contents)
- [Introduction](#introduction)
- [Prerequities](#prerequities)
- [Project Specifications](#project-specifications)
- [Project Architecture](#project-architecture)
- [Setup](#setup)

## Introduction

In this tutorial, we are going to build a simple CLI based application that will help us manage our
own list of books! We are going to create a CLI interface and use SQLite to store data locally.

## Prerequities

In order to follow this tutorial, you will have to be familiar with the following tools and technologies:

- Javascript
- NodeJS
- SQLite

## Project Specifications

We are going to build a simple book gathering application. The primary functions of the application include:

- User should be able to add new books, both individually and in bulk.
- User should be able to edit books, individually or in bulk.
- User should be able to delete books, individually or in bulk.

## Project Architecture

The application uses multiple npm packages to make our life easier to create a CLI based application.
In this case, we will make use of the following NPM packages:

- [commander](https://www.npmjs.com/package/commander)
  - For implementing the UI for the command line.
- [chalk](https://www.npmjs.com/package/chalk)
  - For styling the UI :)
- [sequelize](https://www.npmjs.com/package/sequelize)
  - An ORM to make it easier for us to manage the data.

The basic idea is that commander provides us with an interface to feed onto commands with various
arguements & flags, and then run a relevent function to finish the task. We will use sequelize to
store data into an SQLite database. Chalk is used here for styling the output to look clean and
simple. We will create a simple configuration manager that will help us setup the application.
We can also publish this as a package to NPM.

## Setup

Let's get started with

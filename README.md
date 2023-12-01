# Files Manager
![banner](img/banner.png)

![GitHub repo size](https://img.shields.io/github/repo-size/MulukenMathewos/alx-files_manager)
![GitHub issues](https://img.shields.io/github/issues/MulukenMathewos/alx-files_manager)
![GitHub Repo stars](https://img.shields.io/github/stars/MulukenMathewos/alx-files_manager?logo=github&style=flat)
![GitHub forks](https://img.shields.io/github/forks/MulukenMathewos/alx-files_manager?logo=github&style=falt)
![GitHub commit activity](https://img.shields.io/github/commit-activity/m/MulukenMathewos/alx-files_manager?logo=github)

## Overview
This project is a culmination of key back-end concepts including authentication, Node.js, MongoDB, Redis, pagination, and background processing. The primary objective is to create a simple platform for uploading and viewing files with the following features:

## Features
- User authentication via a token
- List all files
- Upload a new file
- Change permission of a file
- View a file
- Generate thumbnails for images

## Table of Contents
- [Files Manager](#files-manager)
  - [Overview](#overview)
  - [Features](#features)
  - [Table of Contents](#table-of-contents)
  - [Requirements](#requirements)
    - [Applications](#applications)
    - [APIs](#apis)
    - [Environment Variables](#environment-variables)
  - [Installation](#installation)
  - [Usage](#usage)
  - [Tests](#tests)

## Requirements

### Applications

+ Node.js
+ Yarn (the package manager/resource negotiator)

### APIs

+ A Google API should be created with at least an email sending scope and a valid URL (e.g.; `http://localhost:5000/`) should be one of the redirect URIs. The `credentials.json` file should be stored in the root directory of this project.

### Environment Variables

The required environment variables should be stored in a file named `.env` and each line should have the format `Name=Value`. The table below lists the environment variables that will be used by this server:

| Name | Required | Description |
|:-|:-|:-|
| GOOGLE_MAIL_SENDER | Yes | The email address of the account responsible for sending emails to users. |
| PORT | No (Default: `5000`)| The port the server should listen at. |
| DB_HOST | No (Default: `localhost`)| The database host. |
| DB_PORT | No (Default: `27017`)| The database port. |
| DB_DATABASE | No (Default: `files_manager`)| The database name. |
| FOLDER_PATH | No (Default: `/tmp/files_manager` (Linux, Mac OS X) & `%TEMP%/files_manager` (Windows)) | The local folder where files are saved. |

## Installation

+ Clone this repository and switch to the cloned repository's directory.
+ Install the packages using `yarn install` or `npm install`.

## Usage

Start the Redis and MongoDB services on your system and run `yarn start-server` or `npm run start-server`.

## Tests

+ Create a separate `.env` file for the tests named `.env.test` and store the value of the environment variables for the testing event in it.
+ Run `yarn test` or `npm run test` to execute the E2E tests.

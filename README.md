---
title: Astro
description: The basics example astro app, utilizing `serve` to serve the built app
tags:
  - astro
  - serve
---

# Astro Basic

This is a the [astro basic example](https://github.com/withastro/astro/tree/main/examples/basics) that uses [serve](https://www.npmjs.com/package/serve)

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/0768LP?referralCode=ySCnWl)

## ✨ Features

- Astro basic example
- Serve

## 💁‍♀️ How to use

- Install required dependencies with `npm install`
- Start the server for development `npm run dev`

    (The original `start` command has been more appropriately renamed to `dev`)

## ❓ Why use `serve`

By default Railway will use the `start` script defined in package.json to run your app, the problem with that for the default basic example project is that the start script starts a development server
not fit to run on railway, for reasons such as:

 - Starts a file watching development server that's resource intensive
 - Has a tendency for ram to get out of hand (>600mb)
 - Doesn't listen on the railway provided PORT variable
 - Not as stable or performant as `serve`
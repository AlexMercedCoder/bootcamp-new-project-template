## Bootcamp Project Repo Template

This is a template for helping build your project in a coding bootcamp. The main purpose of this is to help you to write quality documentation. Documentation is written in md files using markdown syntax wich you can see [here](https://www.markdownguide.org/basic-syntax/).

## [Product Requirements Document(PRD)](./docs/prd.md)

This document located in the docs folder should be filled out before starting your project to help you think through what your building. 

## Documenting Challenges and Solutions - Issues

Whenever you run into an issue you should create an issue on your repository (you'll issues in the menu at the top of the screen). Create the issue and make comments as you learn new things to solve the problem. This becomes something that can help you and other users in the future.

## Other Files in this template

- Procfile: this file is deployment to Heroku, it tells heroku what command to run to start your application. Usally something like:

```
web: npm start
```

- vercel.json: custom settings for deploying frontend applications to vercel, if deploying a react app using react-router put this in the vercel.json so refershing the deployed page does break things.

```
{
  "version": 2,
  "routes": [
    { "handle": "filesystem" },
    { "src": "/.*", "dest": "/index.html" }
  ]
}
```

- netlify.toml: custom settings deploying a frontend application to netlify, if deploying a react app using react router put this in the netlify.toml

```
[[redirects]]
  from = "/*"
  to = "/index.html"
```

## Making a normal html/css/js app

Just make sude index.html is at the top level of the repo (in the same folder as this readme.md file)

## Making a Backend Node app (expres/koa/fastify)

Make sure the package.json is at the top of this repo and that the start script is defined (heroku will run the start script unless something else specified in the Procfile.

## Making a React App

Set your terminal to the top of this repo (the folder this readme.md is in) and run `npx create-react-app@latest .` which will generate a react app in this folder.

## Deployment

- [Video: Deploy Frontend website to Netlify, Github Pages, Surge, and Heroku](https://www.youtube.com/watch?v=HCDCrjQsEhg)
- [Video: Deploy Frontend to Vercel, AWS Amplify, Firebase, Azure Static](https://www.youtube.com/watch?v=2FVY_lm-mTY)
- [Video: Deploy Frontend website to Render](https://www.youtube.com/watch?v=bB7I-MeI6sY)
- [Video: Deploying NodeJS (Express/Fastify/Koa) to Heroku](https://www.youtube.com/watch?v=hjlAhda-5B4)
- [Blog: Ultimate Guide to deploying nodejs apps to Heroku](https://tuts.alexmercedcoder.com/2021/4/deploying_node_heroku/)
- [Video: Deploying a React App to Netlify](https://www.youtube.com/watch?v=XwOUYUBCaoI)
- [Video: Deploying Python Django to Heroku](https://www.youtube.com/watch?v=Qi2q3c9BNww)
- [Video: Deploying Ruby on Rails to Heroku](https://www.youtube.com/watch?v=n9V_1X8uGZM)

## CORS Issues

- [Overcoming CORS Issues with Severless Functions](https://www.youtube.com/watch?v=wCO4ZLJEDB8)
- [Understanding and Solving Cors](https://www.youtube.com/watch?v=fsMKB7PJoFY)
- [Making A Proxy Server to Overcome Cors](https://www.youtube.com/watch?v=5CFafWpWwxo)

# Deploy rails app using fly.io

## Create rails application

`rails new my_cool_app.rb`

## Integrating fly.io

### Create fly.io profile

Head on to the [fly.io](https://fly.io) and create a new account. Register a credit or debit card as it will be needed to select a region for deployment.

### Install flyctl

`$ cd my_cool_app `

- For mac OS run `$ brew install flyctl ` (if you have the Hombrew installed )
- Install using the install script via curl on LInux and Mac `$ curl -L https://fly.io/install.sh | sh `
- For windows
  `$ powershell -Command "iwr https://fly.io/install.ps1 -useb | iex" `

Once it is installed log into your fly account for authentication via the web.

### Launch

`$ fly launch `

This will create a postgres cluster and prompt you to chose a region. A option to chose a free 100mb Redis would also be given.

### Deploy

`$ fly deploy `

### Preview app

`$ fly open `

## NOTE

- Fly.io utilises and easy to use CLI tool for deployment
- Pay for what you use at comfortable rates. Each app should cost around $4 per month

### Free Plan

- You can host 3 apps for free before you need to start paying.
- Requires a credit card.
- [GoRails video guide for deploying Rails applications to Fly.io](https://www.youtube.com/watch?v=6Zp9y8nF5rE&)
- [Official Documentation](https://fly.io/docs/)

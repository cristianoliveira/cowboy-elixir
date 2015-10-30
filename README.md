# Elixir + Cowboy Hello World
Simple web hello world using Cowboy

## Dependecies:
  - **elixir**: v1.1.1
  - **cowboy**: v1.0.0

## Runing
```Elixir
mix deps.get && mix deps.compile && mix run --no-halt
```
Then access http://localhost:5000

## Your elixir first deploy on Heroku
 - First install Heroku cli

 Instructions here: https://devcenter.heroku.com/articles/heroku-command
 - Prepare the environment
```bash
 heroku create --buildpack "https://github.com/CristianOliveiraDaRosa/heroku-buildpack-elixir.git"
```
- Log into Heroku
```bash
heroku login
```
- Add Heroku as remote

The app name you can get on dashboard.
```bash
heroku git:remote -a <your-app-name>
```

- Finally deploy
```bash
git push heroku master
```

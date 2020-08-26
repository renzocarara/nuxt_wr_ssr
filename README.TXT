
heroku config:set HOST=0.0.0.0 -a morgana-ssr
heroku config:set NODE_ENV=production -a morgana-ssr
heroku config:set NPM_CONFIG_PRODUCTION=false -a morgana-ssr

heroku git:remote -a morgana-ssr

git add .
git commit -m "aggiunto script per heroku"
git push heroku master

# herokutestapp
Test with heroku

using this reference:
https://testdriven.io/blog/deploying-django-to-heroku-with-docker/



# Some notes

```
docker build -t web:latest .
docker run -d --name django-heroku -e "PORT=8765" -e "DEBUG=0" -p 8007:8765 web:latest
docker stop django-heroku
docker rm django-heroku
```

```
heroku logs --tail
```

I'm now at "Postgres Test" 

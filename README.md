# San-Saru AoC Co 2018

## Getting started

To get started with the app, clone the repo and then install the needed gems:

```
$ bundle install --without production
```

Next, migrate the database:

```
$ rails db:migrate
```

on heroku:

    heroku run rails db:migrate
    
#### IMPORTANT: you need to create and admin user!


If the test suite passes, you'll be ready to run the app in a local server:

```
$ foreman start
```

to drop heroku db:
    
    heroku pg:reset DATABASE_URL

config on heroku:

    heroku config:add MAIL_PASSWORD=password12345 MAIL_USERNAME=support@yoururl.com MAIL_DOMAIN=gmail.com SMTP_ADDR=smtp.gmail.com
    
Las invitaciones solo se podran activar si desde la interfaz administrativa se crean:

    las 3 invitaciones iniciales
    se activa el perido de invitaciones en las configuraciones. 
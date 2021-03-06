### Create Laravel Project from Scratch

To make things easier we will use **kool** to install it for you.

```bash
kool docker kooldev/php:7.4 composer create-project --prefer-dist laravel/laravel my-project

cd my-project
```

### Start using kool

Go to the project folder and run:

```bash
$ kool preset laravel
```

**kool preset** basically creates a few configuration files in order to enable you to configure / extend it.

By default laravel preset comes with **mysql** and **redis** configured, you can review how is configured at **docker-compose.yml**.

Also comes with some scripts to bring you up to speed at **kool.yaml**, take a look at the defaults.

By default we always add a script called **setup** to help you setup a project for first time.

```bash
# CAUTION, this script will reset your `.env` file with `.env.example`
$ kool run setup
```

Now you can see your site at **http://localhost**.

Check your **kool.yml** to see what scripts you can run and add more.

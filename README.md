# sidekiq-web

Small standalone rack application to boot up Sidekiq's monitoring console.

## How it works

Start by installing all dependencies:

```bash
$ bundle install
```

Sidekiq will connect by default to the redis instance present at `localhost`, port `6379`. 

If you wish to change this point the `REDIS_URL` environment variable to wherever is useful. Make sure it is a valid Redis URL.

Then just start the daemon and check `http://localhost:9292`!

```bash
$ bundle exec foreman start web
```

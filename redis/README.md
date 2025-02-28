# redis on Fly.io

[Redis](https://redis.io/docs/latest/) is an open source, in-memory data structure store, used as a database, cache, and message broker.

1. Launch the fly application: `$ fly launch --no-deploy` and type y to copy over the fly.toml file.
2. Modify the `redis.conf` file as necessary.
3. Deploy: `$ fly deploy`
4. Allocate shared ipv6 address: `$ fly ips allocate-v6 --private`

Connect via: `your-redis-app-name.internal:6379`

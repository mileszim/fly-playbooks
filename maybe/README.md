# maybe on Fly.io

[Maybe](https://github.com/maybe-finance/maybe) is the OS for your personal finances.

## Instructions

1. Launch the app without deploying: `fly launch --no-deploy`
2. Launch a postgres database for Maybe: `$ fly pg create`
3. Set the connection secrets from the output of the previous command. For example:

   ```bash
   fly secrets set DB_HOST=your-maybe-db.flycast \
                   POSTGRES_DB=maybe \
                   POSTGRES_USER=postgres \
                   POSTGRES_PASSWORD=asdf1234
   ```

4. Generate a random key with: `$ head -c 64 /dev/urandom | od -An -tx1 | tr -d ' \n' && echo`
5. Set `SECRET_KEY_BASE` to that random string: `$ fly secrets set SECRET_KEY_BASE=your-random-string`

Deploy!

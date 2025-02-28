# surrealdb on Fly.io

[surrealdb](https://github.com/surrealdb/surrealdb) is a scalable, distributed, collaborative, document-graph database, for the realtime web.

1. Launch without deploy: `$ fly launch --no-deploy` and type y to use the existing configuration.
2. Configure the username and password via secrets:

   ```bash
   fly secrets set SURREAL_USER="your_username"
   fly secrets set SURREAL_PASS="your_password"
   ```

3. Deploy!

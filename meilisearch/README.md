# meilisearch at Fly.io

[meilisearch](https://github.com/meilisearch/meilisearch) is a lightning-fast search engine API bringing AI-powered hybrid search to your sites and applications.

## Instructions

1. Launch the fly application: `$ fly launch --no-deploy` and type y to copy over the fly.toml file.
2. Generate a random secure key for Meilisearch:

   ```bash
   openssl rand -base64 48
   ```

3. Set `MEILI_MASTER_KEY` secret key to the generate key:

   ```bash
   fly secrets set MEILI_MASTER_KEY=<generated_key>
   ```

4. Deploy!

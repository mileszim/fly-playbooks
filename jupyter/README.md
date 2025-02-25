# jupyter notebook on fly.io

To use your own `requirements.txt`, change the `[build]` section in `fly.toml` to:

```toml
[build]
  dockerfile = 'Dockerfile'
```

An example `requirements.txt` file is included.

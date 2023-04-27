# poetry-git-dependency-repro

The current head has fastapi on [0.95.0](https://github.com/yetanotherion/poetry-git-dependency-repro/blob/ad3afb38d75a2707cd671f64d3a90b860fa8e83c/poetry.lock#L26) when the version *0.95.1* is [available](https://github.com/tiangolo/fastapi/releases)

By editing pyproject.toml and running
```
poetry update fastapi --lock
```

we are able to generate the PR https://github.com/yetanotherion/poetry-git-dependency-repro/pull/4

Instead of running that manually, it would be great if renovate would generate such a PR automatically.

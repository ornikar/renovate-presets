# renovate-presets

Shared configuration for [renovate](https://renovatebot.com/) github bot.

# Installation in your repository

First, make sure renovate has access to the repository.
Then, create the configuration file (don't merge the renovate PR adding this file) :

## If it's an frontend app

> renovate.json

```json
{
  "extends": ["config:js-app", "github>ornikar/renovate-presets:frontend"]
}
```

## If it's a frontend library or monorepo library

> renovate.json

```json
{
  "extends": ["config:js-lib", "github>ornikar/renovate-presets:frontend"]
}
```

## If it's an backend app

> renovate.json

```json
{
    "extends": ["github>ornikar/renovate-presets:backend"]
}
```

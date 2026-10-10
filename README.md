# interactor-weft

The Elixir and OTP control plane of the multiplayer fabric: single-writer actors, a pool reconciler and durable per-actor storage.

## What it is for

It runs one shared 3D world at low latency. A usual game server runs one main loop. weft cuts that loop into parts, and each part runs on its own. The parts together are the mesh. [How weft works](docs/essays/how-it-works.md) explains the whole system in simple words, for a reader who knows neither Elixir nor game engines.

## Build and run

The FoundationDB client library must be installed for the store dependency to compile.

```sh
mix deps.get
mix test
```

## Licence

MIT. See [LICENSE](LICENSE).

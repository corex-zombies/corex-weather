# corex-weather

> Server-authoritative weather and time synchronization.

Part of the [COREX Framework](https://github.com/corex-zombies).

## Install

Drop the `corex-weather` folder into:
```
server-data/resources/[corex]/corex-weather/
```

Make sure it loads after `corex-core`:
```cfg
ensure corex-core
ensure corex-weather
```

## Time API

Server `SetTime(hour, minute)` accepts integer hours 0–23 and minutes 0–59, defaulting omitted minutes to zero. Invalid inputs return false without a state change or broadcast. `GetCurrentTime()` returns hour and minute as two values on both server and client.

## Update safely

Use Weather from the same reviewed COREX revision as its required Core resource
and merge local configuration changes. This workspace README does not imply
that the local candidate has been published.

## Docs
📖 <https://corex-zombies.gitbook.io/corex-docs/reference/weather>

## Community
💬 <https://discord.gg/G95rtnb9sg>

## License
Released under the [MIT License](LICENSE).

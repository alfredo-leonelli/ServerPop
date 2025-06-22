# ServerPop

**Author:** AnotherPanda  
**Version:** 1.0.0  
**Description:** Rust plugin that displays the number of connected players and, optionally, admins via a chat command.

---

## Features

- Displays the total number of connected players in global chat.
- Optionally shows how many of them are admins (configurable).
- Customizable command triggers.

---

## Configuration

A configuration file will be automatically generated at `oxide/config/ServerPop.json` after first load.

```json
{
  "PopCommands": ["pop", "players"],
  "ShowAdminCount": true
}
```

- `PopCommands`: List of commands that players can use to check the server's population status.
- `ShowAdminCount`: If set to `true`, the number of connected admins will be displayed. If `false`, admin info will be omitted.

---

## Usage

Any player can type one of the configured commands (by default `/pop` or `/players`) in the in-game chat.

Example output when `ShowAdminCount` is enabled:

```
There are 12 player(s) connected to the server. Admin(s) online: 2
```

Example output when `ShowAdminCount` is disabled:

```
There are 12 player(s) connected to the server.
```

---

## Notes

- Commands are case-insensitive.
- This plugin does not differentiate between invisible or stealth-admin players.

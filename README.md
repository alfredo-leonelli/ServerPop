# ServerPop

**Version:** 1.0.0  
**Author:** AnotherPanda  
**Description:** Displays the number of connected players and optionally admins via chat command.

---

## Features

- Shows total connected players in chat.
- Optionally includes count of connected admins.
- Customizable chat command triggers.

---

## Configuration

Upon first launch, the plugin will generate the following config file:

```json
{
  "PopCommands": ["pop", "players"],
  "ShowAdminCount": true
}
```

### Config Parameters

| Key              | Type    | Description                                                     |
| ---------------- | ------- | --------------------------------------------------------------- |
| `PopCommands`    | array   | Commands players can use to check server population.            |
| `ShowAdminCount` | boolean | If true, shows count of connected admins in the output message. |

---

## Usage

Players can type `/pop` or `/players` in chat to see the current population.

**Example with `ShowAdminCount = true`:**

```
There are 12 player(s) connected to the server. Admin(s) online: 2
```

**Example with `ShowAdminCount = false`:**

```
There are 12 player(s) connected to the server.
```

---

## Notes

- Commands are case-insensitive.
- Does not detect invisible or stealth-admin players.

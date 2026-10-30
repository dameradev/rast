# Rast for Claude

Manage your Rast website from [Claude Code](https://claude.com/claude-code).
Tell Claude what you want changed and it does the work on your site: rewrite a
page, add a section, upload project photos, update a floor plan or an available
home, reply to a buyer inquiry, adjust forms, bookings or site settings.

Built for the home builders who run their sites on [Rast](https://rast.is).

## Install

In a terminal:

```bash
claude plugin marketplace add dameradev/rast
```

```bash
claude plugin install rast@rast
```

Then start Claude Code (or restart it if it was open).

## Sign in

The first time Claude uses Rast it asks you to connect. In Claude Code, run
`/mcp`, pick **plugin:rast:rast** and choose **Authenticate**. Your browser opens
the Rast portal login: sign in with your normal portal email and password and
approve the consent screen. There is no API key to create or paste.

Claude acts as you, within the sites and roles your portal account already has.
If you manage more than one site, ask Claude to list your sites and pick one.

## Revoke access

In the Rast portal, open **Settings → Connected apps** and revoke the
connection. Claude's next request fails and it asks you to sign in again.

To remove the plugin itself:

```bash
claude plugin uninstall rast@rast
```

## What is in this repo

```
.claude-plugin/marketplace.json   the catalog Claude Code reads
plugins/rast/                     the plugin: one connector URL, an icon, this README's short version
```

The plugin holds no code and no credentials, only the connector address
`https://rast.is/api/mcp`. The tools Claude can use and the guidance it follows
come from the Rast server, so they improve with each Rast release without you
updating anything here.

## Help

Step-by-step guide: <https://rast.is/portal/help/claude>

Also using claude.ai or the Claude desktop app? The same guide shows how to add
Rast there as a custom connector.

## License

MIT

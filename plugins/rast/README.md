# Rast plugin for Claude

Connects Claude to your Rast website through the hosted connector at
`https://rast.is/api/mcp`.

Ask Claude in plain words and it makes the change on your site: rewrite a page,
add a Design Studio section, upload photos, update a floor plan or an available
home, reply to a buyer inquiry, adjust forms, bookings or site settings.

Install in one step from a terminal:

    claude plugin install rast --marketplace dameradev/rast

On first use Claude opens the Rast portal login in your browser. Sign in with
your normal portal email and password and approve the consent screen; there
is no API key to create. Claude acts as you, within the sites and roles your
portal account already has.

Revoke access any time in the portal under **Settings → Connected apps**.

The plugin holds no code or credentials, only the connector URL. Tools, server
instructions and the `site-build` guide come from the server itself, so they
update with each Rast release without a new plugin version.

Help: https://rast.is/portal/help/claude

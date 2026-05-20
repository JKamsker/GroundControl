# groundcontrol CLI

- Version: `generated from source`
- OpenCLI: `0.1-draft`

Command-line reference for `groundcontrol CLI`. Available command areas include authentication, client, config entry, group, project, role, and more.

GroundControl management tool

## Table of Contents

- [Overview](#overview)
- [Root Options](#root-options)
- [Commands](#commands)
  - [audit](#command-audit)
    - [audit get](#command-audit-get)
    - [audit list](#command-audit-list)
  - [auth](#command-auth)
    - [auth login](#command-auth-login)
    - [auth logout](#command-auth-logout)
    - [auth status](#command-auth-status)
  - [client](#command-client)
    - [client create](#command-client-create)
    - [client delete](#command-client-delete)
    - [client get](#command-client-get)
    - [client list](#command-client-list)
    - [client update](#command-client-update)
  - [client-config](#command-client-config)
    - [client-config get](#command-client-config-get)
  - [config](#command-config)
    - [config import](#command-config-import)
    - [config show](#command-config-show)
  - [config-entry](#command-config-entry)
    - [config-entry create](#command-config-entry-create)
    - [config-entry delete](#command-config-entry-delete)
    - [config-entry get](#command-config-entry-get)
    - [config-entry list](#command-config-entry-list)
    - [config-entry update](#command-config-entry-update)
  - [group](#command-group)
    - [group create](#command-group-create)
    - [group delete](#command-group-delete)
    - [group get](#command-group-get)
    - [group list](#command-group-list)
    - [group update](#command-group-update)
  - [project](#command-project)
    - [project create](#command-project-create)
    - [project delete](#command-project-delete)
    - [project get](#command-project-get)
    - [project list](#command-project-list)
    - [project update](#command-project-update)
  - [role](#command-role)
    - [role create](#command-role-create)
    - [role delete](#command-role-delete)
    - [role get](#command-role-get)
    - [role list](#command-role-list)
    - [role update](#command-role-update)
  - [scope](#command-scope)
    - [scope create](#command-scope-create)
    - [scope delete](#command-scope-delete)
    - [scope get](#command-scope-get)
    - [scope list](#command-scope-list)
    - [scope update](#command-scope-update)
  - [snapshot](#command-snapshot)
    - [snapshot get](#command-snapshot-get)
    - [snapshot list](#command-snapshot-list)
    - [snapshot publish](#command-snapshot-publish)
  - [template](#command-template)
    - [template create](#command-template-create)
    - [template delete](#command-template-delete)
    - [template get](#command-template-get)
    - [template list](#command-template-list)
    - [template update](#command-template-update)
  - [token](#command-token)
    - [token create](#command-token-create)
    - [token get](#command-token-get)
    - [token list](#command-token-list)
    - [token revoke](#command-token-revoke)
  - [tui](#command-tui)
  - [user](#command-user)
    - [user create](#command-user-create)
    - [user delete](#command-user-delete)
    - [user get](#command-user-get)
    - [user list](#command-user-list)
    - [user update](#command-user-update)
  - [variable](#command-variable)
    - [variable create](#command-variable-create)
    - [variable delete](#command-variable-delete)
    - [variable get](#command-variable-get)
    - [variable list](#command-variable-list)
    - [variable update](#command-variable-update)

<a id="overview"></a>
## Overview

### CLI Scope

- Top-level command groups: `16`
- Documented commands: `76`
- Leaf commands: `61`

### Available Commands

- [audit](#command-audit) — View audit records
- [auth](#command-auth) — Manage server credentials
- [client](#command-client) — Manage clients
- [client-config](#command-client-config) — Test client configuration resolution
- [config](#command-config) — Manage GroundControl configuration
- [config-entry](#command-config-entry) — Manage configuration entries
- [group](#command-group) — Manage groups
- [project](#command-project) — Manage projects
- [role](#command-role) — Manage roles
- [scope](#command-scope) — Manage scopes
- [snapshot](#command-snapshot) — Manage snapshots
- [template](#command-template) — Manage templates
- [token](#command-token) — Manage personal access tokens
- [tui](#command-tui) — Launch the interactive TUI dashboard
- [user](#command-user) — Manage users
- [variable](#command-variable) — Manage variables


<a id="root-options"></a>
## Root Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --version | — | flag | No | No | Declared | — | Show version information | — |


<a id="commands"></a>
## Commands

<a id="command-audit"></a>
## `audit`

View audit records

### Subcommands

- `get` — Get an audit record by ID
- `list` — List audit records

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-audit-get"></a>
### `audit get`

Get an audit record by ID

#### Arguments

| Name | Required | Arity | Accepted Values | Group | Description |
| --- | --- | --- | --- | --- | --- |
| ID | Yes | 1 | — | — | The audit record ID |

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-audit-list"></a>
### `audit list`

List audit records

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --entity-type | — | <ENTITY_TYPE> | No | No | Declared | — | Filter by entity type | ENTITY_TYPE · required · arity 1 |
| --entity-id | — | <ENTITY_ID> | No | No | Declared | — | Filter by entity ID | ENTITY_ID · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-auth"></a>
## `auth`

Manage server credentials

### Subcommands

- `login` — Log in to a GroundControl server
- `logout` — Clear stored credentials
- `status` — Show current authentication status

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-auth-login"></a>
### `auth login`

Log in to a GroundControl server

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --server-url | — | <SERVER_URL> | No | No | Declared | — | The server URL (Required) | SERVER_URL · required · arity 1 |
| --method | — | <METHOD> | No | No | Declared | — | Authentication method (None, Pat, ApiKey, Credentials) (Required) | METHOD · required · arity 1 |
| --token | — | <TOKEN> | No | No | Declared | — | Personal access token | TOKEN · required · arity 1 |
| --client-id | — | <CLIENT_ID> | No | No | Declared | — | API key client ID | CLIENT_ID · required · arity 1 |
| --client-secret | — | <CLIENT_SECRET> | No | No | Declared | — | API key client secret | CLIENT_SECRET · required · arity 1 |
| --username | — | <USERNAME> | No | No | Declared | — | Username for credential auth | USERNAME · required · arity 1 |
| --password | — | <PASSWORD> | No | No | Declared | — | Password for credential auth | PASSWORD · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-auth-logout"></a>
### `auth logout`

Clear stored credentials

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-auth-status"></a>
### `auth status`

Show current authentication status

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-client"></a>
## `client`

Manage clients

### Subcommands

- `create` — Create a new client
- `delete` — Delete a client
- `get` — Get a client by ID
- `list` — List all clients for a project
- `update` — Update a client

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-client-create"></a>
### `client create`

Create a new client

<a id="command-client-delete"></a>
### `client delete`

Delete a client

<a id="command-client-get"></a>
### `client get`

Get a client by ID

<a id="command-client-list"></a>
### `client list`

List all clients for a project

<a id="command-client-update"></a>
### `client update`

Update a client

<a id="command-client-config"></a>
## `client-config`

Test client configuration resolution

### Subcommands

- `get` — Fetch resolved configuration for a client

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-client-config-get"></a>
### `client-config get`

Fetch resolved configuration for a client

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --client-id | — | <CLIENT_ID> | No | No | Declared | — | The client ID to authenticate with. | CLIENT_ID · required · arity 1 |
| --client-secret | — | <CLIENT_SECRET> | No | No | Declared | — | The client secret to authenticate with. | CLIENT_SECRET · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-config"></a>
## `config`

Manage GroundControl configuration

### Subcommands

- `import` — Import server configuration from a JSON file or paste
- `show` — Display effective GroundControl configuration

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-config-import"></a>
### `config import`

Import server configuration from a JSON file or paste

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --file | — | <FILE> | No | No | Declared | — | Path to a JSON configuration file | FILE · required · arity 1 |
| --paste | — | flag | No | No | Declared | — | Paste JSON configuration interactively | — |
| --yes | — | flag | No | No | Declared | — | Skip confirmation prompt | — |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-config-show"></a>
### `config show`

Display effective GroundControl configuration

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-config-entry"></a>
## `config-entry`

Manage configuration entries

### Subcommands

- `create` — Create a new configuration entry
- `delete` — Delete a configuration entry
- `get` — Get a configuration entry by ID
- `list` — List configuration entries
- `update` — Update a configuration entry

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-config-entry-create"></a>
### `config-entry create`

Create a new configuration entry

<a id="command-config-entry-delete"></a>
### `config-entry delete`

Delete a configuration entry

<a id="command-config-entry-get"></a>
### `config-entry get`

Get a configuration entry by ID

<a id="command-config-entry-list"></a>
### `config-entry list`

List configuration entries

<a id="command-config-entry-update"></a>
### `config-entry update`

Update a configuration entry

<a id="command-group"></a>
## `group`

Manage groups

### Subcommands

- `create` — Create a new group
- `delete` — Delete a group
- `get` — Get a group by ID
- `list` — List all groups
- `update` — Update a group

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-group-create"></a>
### `group create`

Create a new group

<a id="command-group-delete"></a>
### `group delete`

Delete a group

<a id="command-group-get"></a>
### `group get`

Get a group by ID

<a id="command-group-list"></a>
### `group list`

List all groups

<a id="command-group-update"></a>
### `group update`

Update a group

<a id="command-project"></a>
## `project`

Manage projects

### Subcommands

- `create` — Create a new project
- `delete` — Delete a project
- `get` — Get a project by ID
- `list` — List all projects
- `update` — Update a project

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-project-create"></a>
### `project create`

Create a new project

<a id="command-project-delete"></a>
### `project delete`

Delete a project

<a id="command-project-get"></a>
### `project get`

Get a project by ID

<a id="command-project-list"></a>
### `project list`

List all projects

<a id="command-project-update"></a>
### `project update`

Update a project

<a id="command-role"></a>
## `role`

Manage roles

### Subcommands

- `create` — Create a new role
- `delete` — Delete a role
- `get` — Get a role by ID
- `list` — List all roles
- `update` — Update a role

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-role-create"></a>
### `role create`

Create a new role

<a id="command-role-delete"></a>
### `role delete`

Delete a role

<a id="command-role-get"></a>
### `role get`

Get a role by ID

<a id="command-role-list"></a>
### `role list`

List all roles

<a id="command-role-update"></a>
### `role update`

Update a role

<a id="command-scope"></a>
## `scope`

Manage scopes

### Subcommands

- `create` — Create a new scope
- `delete` — Delete a scope
- `get` — Get a scope by ID
- `list` — List all scopes
- `update` — Update a scope

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-scope-create"></a>
### `scope create`

Create a new scope

<a id="command-scope-delete"></a>
### `scope delete`

Delete a scope

<a id="command-scope-get"></a>
### `scope get`

Get a scope by ID

<a id="command-scope-list"></a>
### `scope list`

List all scopes

<a id="command-scope-update"></a>
### `scope update`

Update a scope

<a id="command-snapshot"></a>
## `snapshot`

Manage snapshots

### Subcommands

- `get` — Get a snapshot by ID
- `list` — List snapshots for a project
- `publish` — Publish a new snapshot for a project

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-snapshot-get"></a>
### `snapshot get`

Get a snapshot by ID

#### Arguments

| Name | Required | Arity | Accepted Values | Group | Description |
| --- | --- | --- | --- | --- | --- |
| ID | Yes | 1 | — | — | The snapshot ID |

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --project-id | — | <PROJECT_ID> | No | No | Declared | — | The project ID | PROJECT_ID · required · arity 1 |
| --decrypt | — | flag | No | No | Declared | — | Decrypt sensitive values | — |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-snapshot-list"></a>
### `snapshot list`

List snapshots for a project

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --project-id | — | <PROJECT_ID> | No | No | Declared | — | The project ID to list snapshots for (Required) | PROJECT_ID · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-snapshot-publish"></a>
### `snapshot publish`

Publish a new snapshot for a project

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --project-id | — | <PROJECT_ID> | No | No | Declared | — | The project ID to publish a snapshot for | PROJECT_ID · required · arity 1 |
| --description | — | <DESCRIPTION> | No | No | Declared | — | An optional description for the snapshot | DESCRIPTION · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-template"></a>
## `template`

Manage templates

### Subcommands

- `create` — Create a new template
- `delete` — Delete a template
- `get` — Get a template by ID
- `list` — List all templates
- `update` — Update a template

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-template-create"></a>
### `template create`

Create a new template

<a id="command-template-delete"></a>
### `template delete`

Delete a template

<a id="command-template-get"></a>
### `template get`

Get a template by ID

<a id="command-template-list"></a>
### `template list`

List all templates

<a id="command-template-update"></a>
### `template update`

Update a template

<a id="command-token"></a>
## `token`

Manage personal access tokens

### Subcommands

- `create` — Create a new personal access token
- `get` — Get a personal access token by ID
- `list` — List personal access tokens
- `revoke` — Revoke a personal access token

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-token-create"></a>
### `token create`

Create a new personal access token

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --name | — | <NAME> | No | No | Declared | — | The token name (Required) | NAME · required · arity 1 |
| --expires-in | — | <EXPIRES_IN> | No | No | Declared | — | Token lifetime (e.g. 30d, 6m, 1y). Defaults to 30 days if omitted. | EXPIRES_IN · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-token-get"></a>
### `token get`

Get a personal access token by ID

#### Arguments

| Name | Required | Arity | Accepted Values | Group | Description |
| --- | --- | --- | --- | --- | --- |
| ID | Yes | 1 | — | — | The token ID |

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-token-list"></a>
### `token list`

List personal access tokens

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-token-revoke"></a>
### `token revoke`

Revoke a personal access token

#### Arguments

| Name | Required | Arity | Accepted Values | Group | Description |
| --- | --- | --- | --- | --- | --- |
| ID | Yes | 1 | — | — | The token ID |

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --yes | — | flag | No | No | Declared | — | Skip confirmation prompt | — |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-tui"></a>
## `tui`

Launch the interactive TUI dashboard

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-user"></a>
## `user`

Manage users

### Subcommands

- `create` — Create a new user
- `delete` — Delete a user
- `get` — Get a user by ID
- `list` — List all users
- `update` — Update a user

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-user-create"></a>
### `user create`

Create a new user

<a id="command-user-delete"></a>
### `user delete`

Delete a user

<a id="command-user-get"></a>
### `user get`

Get a user by ID

<a id="command-user-list"></a>
### `user list`

List all users

<a id="command-user-update"></a>
### `user update`

Update a user

<a id="command-variable"></a>
## `variable`

Manage variables

### Subcommands

- `create` — Create a new variable
- `delete` — Delete a variable
- `get` — Get a variable by ID
- `list` — List variables
- `update` — Update a variable

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-variable-create"></a>
### `variable create`

Create a new variable

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --name | — | <NAME> | No | No | Declared | — | The variable name (Required) | NAME · required · arity 1 |
| --scope | — | <SCOPE> | No | No | Declared | — | The variable scope (Global or Project) (Required) | SCOPE · required · arity 1 |
| --group-id | — | <GROUP_ID> | No | No | Declared | — | The group ID (for Global scope) | GROUP_ID · required · arity 1 |
| --project-id | — | <PROJECT_ID> | No | No | Declared | — | The project ID (for Project scope) | PROJECT_ID · required · arity 1 |
| --sensitive | — | flag | No | No | Declared | — | Whether the variable contains sensitive data | — |
| --description | — | <DESCRIPTION> | No | No | Declared | — | The variable description | DESCRIPTION · required · arity 1 |
| --value | — | <VALUE> | No | No | Declared | — | Scoped value (e.g., "default=myval" or "env:prod=prodval"). Repeatable. | VALUE · required · arity 1 |
| --values-json | — | <VALUES_JSON> | No | No | Declared | — | Scoped values as JSON array | VALUES_JSON · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-variable-delete"></a>
### `variable delete`

Delete a variable

#### Arguments

| Name | Required | Arity | Accepted Values | Group | Description |
| --- | --- | --- | --- | --- | --- |
| ID | Yes | 1 | — | — | The variable ID |

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --version | — | flag | No | No | Declared | — | Show version information | — |
| --yes | — | flag | No | No | Declared | — | Skip confirmation prompt | — |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-variable-get"></a>
### `variable get`

Get a variable by ID

#### Arguments

| Name | Required | Arity | Accepted Values | Group | Description |
| --- | --- | --- | --- | --- | --- |
| ID | Yes | 1 | — | — | The variable ID |

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --decrypt | — | flag | No | No | Declared | — | Decrypt sensitive values | — |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-variable-list"></a>
### `variable list`

List variables

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --scope | — | <SCOPE> | No | No | Declared | — | Filter by scope (Global or Project) | SCOPE · required · arity 1 |
| --group-id | — | <GROUP_ID> | No | No | Declared | — | Filter by group ID | GROUP_ID · required · arity 1 |
| --project-id | — | <PROJECT_ID> | No | No | Declared | — | Filter by project ID | PROJECT_ID · required · arity 1 |
| --decrypt | — | flag | No | No | Declared | — | Decrypt sensitive values | — |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

<a id="command-variable-update"></a>
### `variable update`

Update a variable

#### Arguments

| Name | Required | Arity | Accepted Values | Group | Description |
| --- | --- | --- | --- | --- | --- |
| ID | Yes | 1 | — | — | The variable ID |

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --sensitive | — | flag | No | No | Declared | — | Whether the variable contains sensitive data | — |
| --description | — | <DESCRIPTION> | No | No | Declared | — | The new description | DESCRIPTION · required · arity 1 |
| --value | — | <VALUE> | No | No | Declared | — | Scoped value (e.g., "default=myval" or "env:prod=prodval"). Repeatable. | VALUE · required · arity 1 |
| --values-json | — | <VALUES_JSON> | No | No | Declared | — | Scoped values as JSON array | VALUES_JSON · required · arity 1 |
| --version | — | flag | No | No | Declared | — | Show version information | — |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
| --debug | — | <DEBUG> | No | No | Declared | — | Enable debug logging to the console. Use '--debug' for standard or '--debug verbose' or '--debug v' for detailed output. | DEBUG · required · arity 1 |
| --output | — | <OUTPUT> | No | No | Declared | — | Output format: table or json. | OUTPUT · required · arity 1 |
| --no-interactive | — | flag | No | No | Declared | — | Disable interactive prompts and use defaults. | — |

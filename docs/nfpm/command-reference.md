---
title: Command Reference
---

<AUTOGENERATED_TABLE_OF_CONTENTS>

---

## Managing Server

## `setup`

Install a new FiveM server that includes NFive. Running `setup` without specifying a location will use the current directory.

**Example**

```bash
nfpm setup
nfpm setup <location>
```

---

## `start`

Starts the FiveM server process in a new window.

**Example**

```bash
nfpm start
```

---

## `status`

Show the current status of NFive, nfpm and currently installed resources.

**Example**

```bash
nfpm status
```

---

## `self-update`

Downloads and updates the newest NFive Plugin Manager (nfpm).

**Example**

```bash
nfpm self-update
```

---

## `clean-cache`

Remove locally cached NFive Plugin Manager (nfpm) packages.

**Example**

```bash
nfpm clean-cache
```

---

## `rcon`

Connect to a running FiveM server over RCON.

**Example**

```bash
nfpm rcon --host <host> --port <port>
```

---

## Using Plugins

## `search`

Searches [NFive Hub](http://hub.nfive.io/) for NFive Plugins.

**Example**

```bash
nfpm search <plugin>
```

---

## `list`

List currently installed NFive plugins.

**Example**

```bash
nfpm list
```

---

## `install`

Installs a plugin or processes the current lock file.

**Example**

```bash
nfpm install
nfpm install <plugin>
nfpm install <plugin>@<version>
```

---

## `remove`

Remove installed NFive plugins.

**Example**

```bash
nfpm remove 
nfpm remove <plugin>
nfpm remove <plugin>@<version>
```

---

## Developing Plugins

## `scaffold`

Generate the boilerplate code for a new plugin.

**Example**

```bash
nfpm scaffold
```
Scaffold can also optionally pointed to different skeleton files that are either local or remote, here are some examples:
```bash
nfpm scaffold http://site.com/some.zip
nfpm scaffold some_dir/
nfpm scaffold someLocal.zip
nfpm scaffold MyGithub/MyRepo
nfpm scaffold MyGithub/MyRepo#MyBranch
```

See [plugin developmet](sdk/sdk-setup) to learn more.

---

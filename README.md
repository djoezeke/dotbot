# **dotbot** - Minimal Bash-based Dotfile Manager

**dotbot** is a minimalist, single-file bash script for managing dotfiles with support for multiple profiles, backups, and easy configuration.

## Features

- Single bash script, no dependencies
- Install/uninstall dotfile profiles from a GitHub repository
- Config file stores repo URL, username/email, default profile, install path
- Switch between profiles, update, backup, restore
- Colorful, modern output and logging
- Interactive config initialization

## Usage

```bash
dotbot <command> [options] [args]
```

### Commands

- `install [profile]` Install dotfile profile from repo
- `uninstall [profile]` Uninstall dotfile profile
- `config [key] [value]` Update config file
- `help [command]` Show help for command or subcommand
- `update` Update dotfiles
- `upgrade` Update dotbot (not yet implemented)
- `profile [show|switch]` Show or switch dotfile profiles
- `list` List available profiles
- `info` Show current configuration
- `backup` Backup current dotfiles
- `restore` Restore dotfiles from backup
- `version` Show version info

### Options

- `-h, --help` Print help text
- `-v, --version` Print script version
- `-V, --verbose` Verbose logging
- `-i, --interactive` Enable interactive setup

## Example

```bash
# Initialize config interactively
dotbot init

# Install a profile
dotbot install myprofile

# Switch profile
dotbot profile switch anotherprofile

# Backup dotfiles
dotbot backup

# Restore dotfiles
dotbot restore

# Show current config
dotbot info
```

## Documentation

Run `dotbot help <command>` for details on any command.

---

Project: https://github.com/djoezeke/dotbot

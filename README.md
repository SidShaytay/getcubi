# Cubi

**A persistent workspace for your coding agents.**

Cubi gives each project its own isolated environment for coding agents such as Claude Code, Codex and Pi. It is powered by NVIDIA OpenShell. Run `cubi` in a project folder and you get the same environment every time you come back.

## Why use it

- **Live project files.** Your project is shared with the environment. Edits land in your host files immediately.
- **Confined agents.** Agents run inside a microVM by default, or a rootless Podman container, under OpenShell sandbox policy. Your host home directory, credentials and SSH agent are not shared.
- **Settings that persist.** Development tools, agent settings and history stay in the environment between sessions.
- **One environment per project.** Multiple agents and Git worktrees for the same project share it.
- **Stop and start.** Stop an environment to free resources and start it again later. Guest files are kept.
- **SSH access.** Connect a desktop agent over SSH with a generated alias and a pinned host key.

## How it works

```sh
cd /path/to/your/project
cubi             # open or reuse this project's environment
cubi claude      # run Claude Code in it
cubi codex       # run Codex in it
cubi pi          # run Pi in it
cubi info        # show the SSH host and guest folder for a desktop agent
cubi stop        # stop the environment and keep its files
cubi start       # start it again
```

Host account credentials are not copied into the environment. Sign in to your agents inside it, or use your desktop client's supported flow.

## Availability

Cubi is not released yet. There is no install command today. Release builds will appear on the [releases page](https://github.com/SidShaytay/getcubi/releases) with installation instructions.

Linux x86-64 comes first. macOS and Windows are planned.

## Feedback

Questions, bug reports and feature requests are welcome in [issues](https://github.com/SidShaytay/getcubi/issues). A short overview is also available on the [project page](docs/index.html).

## License

Cubi is free for personal, noncommercial use. Organizations and commercial use need a license. Full terms will ship with each release. For licensing, [open an issue](https://github.com/SidShaytay/getcubi/issues/new?title=Licensing%20inquiry) and we will be glad to help.

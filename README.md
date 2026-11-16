# Cubi

**A persistent workspace for your coding agents.**

Cubi gives each project its own reusable environment, powered by NVIDIA OpenShell. Your project files stay live on your machine, while your agents work with development tools and persistent guest-local settings.

## Download status

**Binary releases and the installer are in preparation.** There is no supported public installation command yet. You do not need to clone this repository to use a future release; it contains public documentation and distribution materials, not the Cubi implementation.

- [View releases](https://github.com/SidShaytay/getcubi/releases)
- [Read the product overview](docs/index.html)
- [Report a problem or request a feature](https://github.com/SidShaytay/getcubi/issues)

Linux x86-64 is the initial target. macOS and Windows support are planned and are not available yet. Exact Linux requirements and supported distributions will accompany the first qualified binary release.

## The intended experience

Once the first supported release is available, install its verified binary using the published instructions. Then open a terminal in your project and run:

```sh
cd /path/to/your/project
cubi
```

Cubi will prepare or reopen that project's workspace. Project edits affect the host files immediately. Host account credentials are not automatically copied into the workspace; authenticate using the release's supported instructions.

Installation, first-launch requirements and update instructions will be published with the release. Package-manager installations will use their package manager for updates. Do not use unannounced install commands or third-party packages claiming to be official Cubi releases.

## License and organizational use

Cubi is proprietary, closed-source software. Free use is limited to individuals acting privately for personal, noncommercial purposes. Use by or on behalf of an organization—including a nonprofit, school or research institution—and commercial use require a separate written license. Full terms and third-party notices will accompany each release.

For an organizational or commercial licensing inquiry, [open an issue](https://github.com/SidShaytay/getcubi/issues/new?title=Licensing%20inquiry). Share only a general description of the intended use; do not post private contact, billing or account information publicly.

## Website publication

The static landing page is in `docs/index.html`; it uses no build tool or external assets. An owner can enable GitHub Pages in **Settings → Pages**, select **Deploy from a branch**, choose **main** and **/docs**, then save. Pages is not automatically enabled by adding these files. The expected project URL after activation is `https://sidshaytay.github.io/getcubi/`.

Only public product materials belong in this repository. Release archives must contain approved binary distribution files and required notices, without implementation source or private development history.

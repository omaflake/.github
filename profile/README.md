<p align="center">
  <img src="assets/omaflake-banner.png" alt="omaflake – clean, disposable NixOS and macOS VMs on Mac and Linux" width="100%">
</p>

**Clean, disposable NixOS and macOS virtual machines on Mac and Linux – one click away.**

[Download](https://omaflake.app) · [Documentation](https://omaflake.dev) · [Recipes](https://github.com/omaflake/recipes) ·
[Discussions](https://github.com/orgs/omaflake/discussions)

omaflake builds VM templates from **recipes** you declare in Nix and runs disposable VMs from them – from an app (the menu
bar on a Mac, a native window on Linux), `omaf ui` or the `omaf` CLI. Templates never change: *reset* throws a VM's state away and starts over.

- **Mac and Linux:** a Mac with Apple silicon runs NixOS and macOS guests; a Linux PC with Nix (or NixOS), x86_64 or
  aarch64, runs NixOS guests with KVM.
- **Two guest kinds:** NixOS on QEMU (3D with virglrenderer) and macOS on Virtualization.framework – the macOS base is
  installed from Apple's restore image without manual steps.
- **Recipes from sources:** the official catalog, other GitHub repositories (also private), or a local folder – share
  recipes, not machines.
- **Integrated:** sound and microphone, shared clipboard with text and images, the host's camera in NixOS guests,
  shared folders, dynamic resolution, ephemeral VMs.
- **Portable:** export VMs, templates and recipes as packages to an external disk and back, or run a VM from there.
- **Doctor:** checks what the computer brings and names the fix; on a Mac it sets up Nix, nix-darwin and the Linux
  builder by click.

| Repository | What |
|---|---|
| [omaflake](https://github.com/omaflake/omaflake) | the apps for macOS and Linux, the `omaf` CLI, the macOS runner, the patched QEMU and the image flake |
| [recipes](https://github.com/omaflake/recipes) | the official recipe catalog – and the template for your own recipe source |
| [website](https://github.com/omaflake/website) | omaflake's landing page |

### The name

```
OMAkase + FLAKE → omaflake
```

*Omakase* is Japanese for "I'll leave it to you": at a sushi bar, the chef chooses. Omarchy, the opinionated Arch
Linux setup, took its name from it, and omaflake follows – a recipe chooses a whole system for you, ready to use. A
*flake* is Nix's unit of reproducible code: it pins exactly what goes into a system, so the result is the same every
time. Together: the chef's choice, reproducible.

> **Status:** alpha, unsigned – download at [omaflake.app](https://omaflake.app). Runs on a Mac with Apple silicon and macOS 27, or on
> Linux with Nix (NixOS guests only).

<sub>omaflake is free software (AGPL-3.0-or-later; its recipes MIT) and a project of <a href="https://falkoss.org">falkOSS</a> – Falcon Lake Open Source Software gUG (haftungsbeschränkt) i. G., from Falkensee.</sub>

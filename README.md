# Claude Launcher — downloads

Created by [freecodespot.com](https://freecodespot.com) · MIT license (see `LICENSE`).

Claude Launcher is a Windows desktop app that runs your [Claude Code](https://claude.com/claude-code)
projects from one window: a project registry (`projects.json`), workspaces to group projects
(for example *Work* and *SideQuest*), one embedded PowerShell terminal tab per project, a usage
panel, crash recovery (`claude --resume` after an unexpected exit) and an automatic session
hand-over when a tab is closed.

This repository only hosts the **release builds**. Download the latest version from the
[Releases](../../releases/latest) page.

## Install

1. Download `ClaudeLauncher.exe` (portable, self-contained, no .NET install needed) or the `.zip`
   from the latest release.
2. Put it anywhere, for example next to a `claude-config` folder, and run it. On the first run it
   either finds an existing `claude-config` folder or offers to generate one from templates.
3. Optional: check the file against `SHA256SUMS.txt` with `certutil -hashfile ClaudeLauncher.exe SHA256`.

The exe is not code-signed, so Windows SmartScreen may show "Windows protected your PC" the first
time; choose *More info* → *Run anyway*.

## Requirements

- Windows 10 version 1809 or later, 64-bit.
- [Claude Code](https://claude.com/claude-code) installed (`claude` on the PATH).
- Windows PowerShell 5.1 (included in Windows) or PowerShell 7.

## Support

Open an issue in this repository. Please include the log file from
`%LOCALAPPDATA%\ClaudeLauncher\logs\`.

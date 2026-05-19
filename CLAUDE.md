# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository contents

This repository currently contains only plain-text allowlists — no source code, build system, package manifest, or tests.

- `good_domains.txt` — one domain per line (e.g. `google.com`).
- `good_ips.txt` — one IP address per line (e.g. `8.8.8.8`).
- `README.md` — stub, contains only the repo name.

## Conventions for the data files

- One entry per line, no comments, no blank lines between entries, trailing newline at end of file.
- `good_domains.txt` holds bare hostnames only (no scheme, no path, no port).
- `good_ips.txt` holds bare IPv4 addresses (no CIDR, no port).
- When adding entries, append to the end of the file rather than reordering existing lines, so diffs stay minimal.

## Notes

There are no commands to build, lint, or test. If a future change introduces code, update this file with the relevant workflow.

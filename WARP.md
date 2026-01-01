# WARP.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

## Project Overview

This is a TIL (Today I Learned) repository that uses markdown files for documentation. The repository follows rolasnajera's open source guidelines and uses a dual MIT + Apache 2.0 license.

Future plans include integrating Markdoc or Docusaurus for enhanced documentation capabilities.

## Repository Structure

This is a template repository with the following key files:
- `README.md` - Project overview and template instructions
- `CONTRIBUTING.md` - Contribution guidelines and workflow
- `CODE_OF_CONDUCT.md` - Community standards
- `CHANGELOG.md` - Version history
- `.github/` - Issue templates, PR templates, and CODEOWNERS
- `release.toml` - Release automation configuration
- `.modifymergify.yml` - Mergify automation for PRs

## Development Commands

Since this is primarily a markdown documentation repository, there are no build or test commands currently configured. When Markdoc or Docusaurus is added, typical commands will include:
- Build documentation site
- Run development server
- Lint markdown files

## Markdown Standards

- Follow markdownlint rules (see inline comments in README.md)
- MD041: Allow files without first line heading (when appropriate)
- MD033: Inline HTML is allowed where necessary
- Use proper formatting and structure for readability

## Contribution Workflow

1. Fork the repository
2. Create a feature branch
3. Make changes (ensure markdown is properly formatted)
4. Open a PR with clear description
5. PRs require 1 approval before auto-merge
6. Auto-merge occurs when CI passes (see `.modifymergify.yml`)

## Release Process

Releases use `cargo-release` with configuration in `release.toml`:
- Updates CHANGELOG.md automatically
- Creates git tags
- Replaces version placeholders

When creating releases, ensure CHANGELOG.md has been updated with relevant changes under the `Unreleased` section.

## Commit Messages

All commits made by Warp should include:
```
Co-Authored-By: Warp <agent@warp.dev>
```

## Licensing

All contributions must be dual-licensed under MIT OR Apache 2.0. This is non-negotiable for rolasnajera projects.

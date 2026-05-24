# Contributing to Okudagram

Thank you for your interest in contributing! This document outlines the process for contributing to the project. For end-user documentation, see [README.md](./README.md).

## Code of Conduct

By participating in this project, you agree to maintain a respectful and inclusive environment. Be kind, constructive, and professional in all interactions.

## Reporting Bugs

Bugs are tracked as GitHub issues using the [bug report template](https://github.com/Jalad25/okudagram/issues/new?template=bug_report.yml), which prompts for the reproduction steps, version info, and other details needed to triage the issue.

Before opening a new bug report:

- Search [existing issues](https://github.com/Jalad25/okudagram/issues) to see if it has already been reported.
- Make sure you are running the latest version of the theme and the minimum required version of Obsidian.
- Try to reproduce the bug in a clean vault with other plugins disabled or removed.

## Suggesting Enhancements

Feature requests are tracked as GitHub issues using the [feature request template](https://github.com/Jalad25/okudagram/issues/new?template=feature_request.yml). The template focuses on the *problem* you're trying to solve before the proposed solution.

Before opening an issue, check the [ROADMAP.md](ROADMAP.md) to make sure your idea isn't already planned or out of scope for this theme, and check the [milestones page](https://github.com/Jalad25/okudagram/milestones) to make sure it isn't already scheduled for a release.

If your idea is still in an early stage and you'd like to discuss it before filing a formal request, open an [Ideas discussion](https://github.com/Jalad25/okudagram/discussions) instead.

Accepted feature requests are assigned a [milestone](https://github.com/Jalad25/okudagram/milestones) (e.g. `v2.3.0`) indicating which release they're planned for. Issues without a milestone have not yet been scheduled. They may still be accepted, but no release has been committed to.

## Questions and Discussion

For usage questions, styling help, or sharing how you use the theme, please open a [discussion](https://github.com/Jalad25/okudagram/discussions) rather than an issue. Discussion categories include Q&A, Ideas, and Show & Tell, each with its own template.

## Contributing Code

### Before you start...

- **Check the [ROADMAP.md](ROADMAP.md)** to make sure the same change isn't already planned.
- **Check the [milestones page](https://github.com/Jalad25/okudagram/milestones)** to see which release an issue is scheduled for. If you'd like to work on an issue, comment on it before starting so it can be confirmed available and not already in progress by someone else.
- **Open an issue or discussion** for non-trivial changes so we can agree on the approach. Small fixes (typos, doc improvements, obvious bugs) can skip this.
- **Scope each pull request to one issue, bug, or feature**. Bundled changes are harder to review.

### Once you are ready to edit...

1. **Fork** the repository and create your branch from `main`.
2. **Make your changes** to `theme.css` in a clear, focused commit history.
3. **Follow the style guide** below.
4. **Test your changes** in a local Obsidian vault: copy `manifest.json` and `theme.css` into `<vault>/.obsidian/themes/Okudagram/`, then reload Obsidian and verify the affected UI surfaces. Note that themes can break in non-obvious ways across Obsidian versions, so test against the current public release.
5. **Update documentation** (README.md) if your changes affect user-facing behavior or scope.

### Creating a Pull Request

When creating a pull request you'll be met with a default pull request template. It includes a list of template names that can be appended to the pull request URL to create a PR using one of the specialized templates. If you are unsure of which template to use, the default is fine. Fill out the chosen template and select **Create pull request** when you are ready.

#### Pull Request Templates

For more specific changes, you can use one of the specialized templates:

| Type of change | Template URL parameter |
|---|---|
| New feature | [`?template=feature.md`](https://github.com/Jalad25/okudagram/compare/main...main?template=feature.md&quick_pull=1) |
| Bug fix | [`?template=bugfix.md`](https://github.com/Jalad25/okudagram/compare/main...main?template=bugfix.md&quick_pull=1) |
| Documentation | [`?template=docs.md`](https://github.com/Jalad25/okudagram/compare/main...main?template=docs.md&quick_pull=1) |
| Refactor | [`?template=refactor.md`](https://github.com/Jalad25/okudagram/compare/main...main?template=refactor.md&quick_pull=1) |

## Style

- Match the existing formatting in `theme.css` (2-space indent, nested selectors where they help readability).
- Use the existing palette custom properties (`--okudagram-peach`, etc.) rather than hardcoding hex values.
- Avoid `!important` unless you've confirmed Obsidian's default rule can't be beaten by specificity alone.
- Avoid `:has`, unless absolutely necessary.
- Dark mode only! See the note in the [README.md](README.md). Don't add `.theme-light` rules.

## License

By contributing to this project you agree that your contributions will be licensed under the [GNU General Public License v3.0](LICENSE).
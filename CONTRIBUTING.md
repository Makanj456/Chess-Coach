# Contributing

Thank you for contributing to Chess Coach.

## Creating an issue

Use the appropriate issue template:

- **Feature or user story** for new behavior or functionality
- **Bug report** for reproducible problems or unexpected behavior

Give the issue a clear title that describes the requested change or problem.

## Branch names

Create branches from `main` using the issue title converted to lowercase `snake_case`.

```text
<issue_title_in_snake_case>
```

Examples:

- Issue: “Add move history” → `add_move_history`
- Issue: “Fix login timeout” → `fix_login_timeout`

## Labels

Use labels to describe the kind of work and its current status.

### Work type

- `bug` — Incorrect or unexpected behavior
- `feature` — New functionality
- `documentation` — Documentation-only changes

### Status

- `status:todo` — Ready to be worked on
- `status:in-progress` — Work is underway
- `status:ready-for-review` — Ready for a pull request or review
- `status:blocked` — Cannot proceed until another issue or dependency is resolved

Keep only the current status label applied.

## Pull requests

Create pull requests against `main` and use the repository pull request template.

- Link the related issue with `Closes #n`.
- Keep pull requests focused on one issue.
- Update or add tests for behavioral changes.
- Include screenshots or recordings for visual changes.
- Explain any migrations, configuration changes, or deployment steps.

## Definition of done

Work is done when all applicable criteria are met:

- The implementation satisfies the issue's acceptance criteria.
- The change works end to end.
- Data survives a page reload when persistence is relevant.
- Errors show a readable message instead of a blank or broken screen.
- Tests are added or updated for the behavior.
- Documentation is updated when needed.
- The pull request passes CI and required reviews.
- The pull request is merged into `main`.

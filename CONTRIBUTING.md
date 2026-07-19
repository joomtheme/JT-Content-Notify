# Contributing to JT Content Notify

Thank you for helping improve JT Content Notify.

## Before opening an issue

- Search existing issues first.
- Confirm the problem still exists in the latest release.
- Test with Joomla core Cassiopeia when the problem appears template-related.
- Check both guest and logged-in behaviour when the problem concerns read status.

## Bug reports

A useful bug report includes:

- JT Content Notify version
- Joomla version
- PHP version
- Database type and version
- Template name
- Browser and version
- Guest or logged-in user
- Selected module settings
- Clear reproduction steps
- Expected result
- Actual result
- Relevant Joomla logs or browser console errors

Do not post credentials, private URLs, personal data, or security-sensitive details in public issues.

## Feature requests

Explain:

- The problem or workflow the feature would improve
- The expected Joomla-native behaviour
- Whether the feature affects the component, module, ACL, routing, pagination, multilingual filtering, or read state
- Any compatibility concerns

## Pull requests

1. Fork the repository.
2. Create a focused branch.
3. Keep each pull request limited to one logical change.
4. Follow Joomla coding conventions.
5. Preserve Joomla MVC and dependency-injection patterns.
6. Use Joomla Web Asset Manager for JavaScript and assets.
7. Use Bootstrap 5 and Joomla core classes where possible.
8. Do not modify Joomla core files.
9. Keep English and Turkish language files synchronized.
10. Update manifests, changelog, and release metadata when required.

## Required checks

Before opening a pull request:

- Run PHP syntax checks on all PHP files.
- Validate all XML and JSON files.
- Verify JavaScript syntax.
- Test installation and upgrade on a clean Joomla site.
- Test uninstall behaviour.
- Test ACL with a non-Super-User account.
- Test guest and logged-in read-state behaviour.
- Test multilingual filtering when applicable.
- Run JED Checker.
- Confirm every PHP file contains a GPL-compatible license header.

## Commit messages

Use clear, imperative commit messages, for example:

```text
Fix guest read-state synchronisation
Add pagination limit option
Update Turkish language strings
```

## License

By contributing, you agree that your contribution will be distributed under the GNU General Public License version 2 or later.

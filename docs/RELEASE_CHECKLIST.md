# Release Checklist

Use this checklist before publishing a JT Content Notify release.

## Version consistency

Update the version in:

- Package manifest
- Component manifest
- Module manifest
- Administrator technical information
- `updates/update.xml`
- `updates/changelog.xml`
- `CHANGELOG.md`
- README release examples when necessary

## Package checks

- Build `com_jtcontentnotify.zip`
- Build `mod_jtcontentnotify.zip`
- Build `pkg_jtcontentnotify-x.y.z.zip`
- Verify all ZIP archives can be opened
- Confirm package installation on a clean Joomla site
- Confirm upgrade from the previous version
- Confirm uninstall succeeds cleanly

## Static checks

- PHP syntax check
- XML validation
- JSON validation
- JavaScript syntax check
- GPL-compatible header in every PHP file
- `_JEXEC` protection in every executable PHP file
- JED Checker scan

## Functional checks

- Notification badge count
- Dropdown opening and alignment
- Mark all as read
- Guest `localStorage` state
- Logged-in database state
- Category and child-category filters
- ACL and access levels
- Multilingual filtering
- Scheduled publishing
- View All pagination
- Component Options and Permissions
- Cassiopeia frontend
- Atum administrator interface

## GitHub release

1. Create tag `vX.Y.Z`.
2. Create release title `JT Content Notify vX.Y.Z`.
3. Upload `pkg_jtcontentnotify-X.Y.Z.zip`.
4. Calculate the final SHA-256 checksum.
5. Update `updates/update.xml` with:
   - version
   - release download URL
   - SHA-256
6. Confirm the raw update XML loads publicly.
7. Confirm Joomla detects the update.

Never replace a published release asset without also updating its SHA-256 value.

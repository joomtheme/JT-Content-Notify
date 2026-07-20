# Changelog

All notable changes to JT Content Notify are documented here.

## [1.0.8] - 2026-07-20

### Added

* Dedicated Joomla menu item type for the frontend notification centre
* Joomla Privacy plugin for exporting and removing registered-user read-state data
* System cleanup plugin for removing orphaned state records when users or module instances are deleted
* MySQL, MariaDB, and PostgreSQL update schema support
* Mark all as read action on the paginated View All page
* Read-state updates when opening notification articles from the View All page
* Server-side fallback URL for the View All link

### Changed

* Preserved the active `Itemid`, language, and menu context in notification AJAX requests
* Applied module publication dates, language, access level, enabled state, and menu assignments to AJAX access validation
* Synchronised guest `localStorage` read state between the dropdown and View All page
* Applied the module's category and date display settings to the View All page
* Moved frontend presentation styles into Joomla Web Asset Manager assets
* Replaced the hard-coded administrator version number with dynamically loaded extension metadata
* Paused automatic refresh while the browser tab is hidden
* Prevented overlapping notification AJAX requests
* Improved package metadata for Joomla 6.1 and PHP 8.3 requirements

### Fixed

* Guest notifications appearing unread again after opening the View All page
* Notification articles remaining unread after being opened from the View All page
* Incorrect article routing on multilingual and menu-assigned pages
* Access to notification data from unpublished, expired, language-mismatched, or incorrectly assigned module instances
* View All links becoming unusable when JavaScript or AJAX loading failed
* Concurrent read-state writes causing duplicate database-key conflicts
* Category and date visibility settings being ignored on the View All page

### Security

* Replaced public exception details with generic JSON error responses
* Added server-side exception logging for failed AJAX requests
* Strengthened module-context, ACL, publication, language, and menu-assignment validation
* Retained Joomla CSRF token validation for all read-state changes

## [1.0.7] - 2026-07-19

### Added

- Support and Resources card in the administrator component
- GitHub update server and Joomla changelog integration
- JED-compatible package language metadata
- GPL-compatible license headers across PHP files
- GitHub, JoomTheme, and JED support links

### Changed

- Refined and compacted the administrator support card
- Improved package manifest compatibility with JED Checker
- Kept update-server `<element>` metadata only in the update manifest

### Fixed

- Package language file detection
- Invalid package manifest `<element>` node
- Update server metadata and package checksum consistency

## [1.0.4]

### Added

- Joomla core `ListModel` pagination on the View All page
- Configurable articles-per-page setting

## [1.0.3]

### Fixed

- View All unread indicator size and alignment
- Category alignment beneath article titles

## [1.0.2]

### Added

- Component Options and Permissions
- Joomla ACL actions for management and configuration

### Fixed

- Unread indicator rendering as a true circle

## [1.0.1]

### Changed

- Improved dropdown width and responsive behaviour
- Refined notification row layout and accessibility
- Improved English and Turkish language strings

## [1.0.0]

- Initial release
- Core `com_content` integration
- Frontend notification bell and unread counter
- Dropdown notification list
- Logged-in and guest read-state support
- Mark all as read

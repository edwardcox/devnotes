# Changelog

All notable changes to Dev Notes will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [3.5.0] - 2024-12-20

### Added
- 🌓 Complete theme system with light and dark modes
- Theme toggle switch in header with smooth animations
- Keyboard shortcut `Ctrl/Cmd + D` for quick theme switching
- Automatic system theme detection on first load
- Theme preference persistence in localStorage
- Visual notifications when theme changes
- Optimized styles for both light and dark themes
- Theme-aware syntax highlighting

### Changed
- Improved contrast ratios for better accessibility
- Enhanced shadow effects per theme
- Updated welcome note with theme documentation

### Fixed
- Code preview background colors in light mode
- Category badge visibility in different themes

## [3.4.0] - 2024-12-20

### Added
- 🎨 Custom category management system
- Create unlimited custom categories with names, icons, and colors
- Edit existing category properties (icon, name, color)
- Delete categories (with automatic note reassignment)
- "Manage" button in sidebar for category administration
- Color picker with 12 preset colors
- Restore default categories option
- Category persistence in localStorage
- Keyboard shortcut `Ctrl/Cmd + M` for category management

### Changed
- Categories now support custom colors
- Category badges display with dynamic colors
- Improved category filter visual feedback

### Fixed
- Category assignment for imported notes
- Category colors in note list display

## [3.3.0] - 2024-12-20

### Added
- ⌨️ Comprehensive keyboard shortcuts system
- Quick note creation with `Ctrl/Cmd + N`
- Save confirmation with `Ctrl/Cmd + S`
- Toggle Edit/Preview with `Ctrl/Cmd + E`
- Search focus with `Ctrl/Cmd + /`
- Navigation with `Alt + Arrow keys`
- Delete note with `Shift + Delete`
- Focus controls for title, editor, and tags
- Keyboard shortcuts help modal (press `?`)
- Visual action notifications
- Keyboard hint in bottom corner

### Changed
- Improved focus management throughout app
- Enhanced keyboard navigation flow
- Better visual feedback for all actions

### Fixed
- Focus trap issues in modals
- Keyboard navigation in filtered lists

## [3.2.0] - 2024-12-20

### Added
- 🏷️ Categories and tags organization system
- 8 default categories (API, Config, Snippet, Docs, Notes, Security, Database, Other)
- Color-coded category badges
- Category filtering with note counts
- Custom tags with add/remove functionality
- Tag search capability
- Visual category indicators on note cards
- Enhanced search includes tags

### Changed
- Search now covers titles, content, and tags
- Improved note card layout with category badges
- Better visual hierarchy in note list

### Fixed
- Search performance with large note collections
- Category filter state persistence

## [3.1.0] - 2024-12-20

### Added
- 📝 Full markdown support with live preview
- Rich text formatting (headers, lists, tables, quotes)
- Markdown syntax highlighting in code blocks
- Task lists with checkboxes
- Table rendering with styling
- Link support with hover effects
- Inline code and code block formatting
- Horizontal rules and blockquotes

### Changed
- Enhanced preview mode for markdown
- Improved typography and spacing
- Better code block integration

### Fixed
- Markdown parsing edge cases
- Preview mode scrolling issues

## [3.0.0] - 2024-12-20

### Added
- 🎨 Syntax highlighting for 15+ programming languages
- Language selector dropdown for each note
- Preview mode for formatted code
- Toggle between Edit and Preview modes
- Support for JavaScript, Python, Java, Go, Rust, SQL, and more
- Prism.js integration for highlighting

### Changed
- Note structure includes language property
- Improved code display formatting
- Better monospace font handling

### Fixed
- Code formatting in preview mode
- Language detection for imported notes

## [2.0.0] - 2024-12-20

### Added
- 💾 Persistent storage using localStorage
- Import/Export functionality for backup
- Storage status indicator
- Note size tracking
- Storage usage display
- Fallback to in-memory storage
- Drag-and-drop import support

### Changed
- Complete storage layer rewrite
- Improved data persistence
- Better error handling

### Fixed
- Storage quota exceeded handling
- Import validation issues

## [1.0.0] - 2024-12-20

### Added
- Initial release of Dev Notes
- Single-file HTML application
- Two-column responsive layout
- Basic note CRUD operations
- Search functionality
- Auto-save feature
- Mobile responsive design
- Welcome note for new users

### Core Features
- Create, edit, and delete notes
- Real-time search
- Automatic saving
- Responsive design
- Zero dependencies

---

## Version Naming Convention

- **Major (X.0.0)** - Significant architecture changes or breaking changes
- **Minor (0.X.0)** - New features and enhancements
- **Patch (0.0.X)** - Bug fixes and minor improvements

## Upgrade Guide

### From v2.x to v3.x
- Notes automatically migrate with default language set to "plaintext"
- No manual intervention required

### From v3.x to v3.4+
- Categories are automatically assigned to existing notes
- Custom categories are saved separately from notes

### From v3.4 to v3.5
- Theme defaults to dark mode or system preference
- No migration needed for existing data
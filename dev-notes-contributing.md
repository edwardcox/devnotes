# Contributing to Dev Notes

First off, thank you for considering contributing to Dev Notes! It's people like you that make Dev Notes such a great tool for developers. 🎉

## 📋 Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Setup](#development-setup)
- [Project Structure](#project-structure)
- [Style Guidelines](#style-guidelines)
- [Commit Guidelines](#commit-guidelines)
- [Pull Request Process](#pull-request-process)

## 📜 Code of Conduct

### Our Pledge

We are committed to providing a friendly, safe, and welcoming environment for all contributors, regardless of experience level, gender identity, sexual orientation, disability, personal appearance, race, ethnicity, age, religion, or nationality.

### Expected Behavior

- Be respectful and inclusive
- Welcome newcomers and help them get started
- Focus on what is best for the community
- Show empathy towards other community members

## 🤝 How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check existing issues to avoid duplicates. When creating a bug report, include:

1. **Clear Title** - Summarize the issue
2. **Description** - What happened vs. what you expected
3. **Steps to Reproduce** - Detailed steps to reproduce the issue
4. **Environment** - Browser version, OS, Dev Notes version
5. **Screenshots** - If applicable
6. **Console Errors** - Any JavaScript errors

**Example:**
```markdown
**Title:** Notes fail to save in Firefox

**Description:** When creating a new note in Firefox 95, the save indicator shows but the note isn't persisted after refresh.

**Steps:**
1. Open Dev Notes in Firefox 95
2. Create a new note
3. Add content
4. Refresh the page
5. Note is missing

**Environment:** Firefox 95.0, Windows 11, Dev Notes v3.5
```

### Suggesting Enhancements

Enhancement suggestions are welcome! Please provide:

1. **Use Case** - Why is this enhancement needed?
2. **Current Behavior** - What happens now?
3. **Desired Behavior** - What should happen?
4. **Possible Implementation** - Ideas on how to implement it

### Code Contributions

1. **Find an Issue** - Look for issues labeled `good first issue` or `help wanted`
2. **Comment** - Let others know you're working on it
3. **Fork & Branch** - Create a feature branch from `main`
4. **Code** - Make your changes
5. **Test** - Ensure everything works
6. **Pull Request** - Submit your changes

## 🛠️ Development Setup

Since Dev Notes is a single HTML file, setup is minimal:

1. **Fork the Repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/dev-notes.git
   cd dev-notes
   ```

2. **Open in Browser**
   - Direct: Open `dev-notes-v3.5.html` in your browser
   - With server: `python -m http.server 8000` then visit `localhost:8000`

3. **Edit and Refresh**
   - Make changes to the HTML file
   - Refresh browser to see changes

### Testing Checklist

Before submitting, test:
- [ ] Create, edit, delete notes
- [ ] Categories and tags
- [ ] Import/Export
- [ ] Theme switching
- [ ] Keyboard shortcuts
- [ ] Mobile responsiveness
- [ ] Different browsers

## 📁 Project Structure

```
dev-notes-v3.5.html
├── HTML Structure (lines 1-850)
│   ├── Header
│   ├── Sidebar
│   ├── Canvas Area
│   └── Modals
├── CSS Styles (lines 850-1650)
│   ├── Variables
│   ├── Base Styles
│   ├── Components
│   ├── Theme System
│   └── Responsive
└── JavaScript (lines 1650-2500)
    ├── Storage Manager
    ├── Note Operations
    ├── UI Functions
    ├── Shortcuts
    └── Initialization
```

## 🎨 Style Guidelines

### HTML/CSS
- Use semantic HTML5 elements
- Follow BEM-like naming for classes
- Keep CSS variables in `:root`
- Mobile-first responsive design
- Support both light and dark themes

### JavaScript
- Use meaningful variable names
- Comment complex logic
- Keep functions small and focused
- Handle errors gracefully
- Maintain backward compatibility

**Example:**
```javascript
// Good
function createNewNote() {
    const note = {
        id: Date.now(),
        title: "Untitled Note",
        content: "",
        // ... clear structure
    };
    // ... rest of function
}

// Avoid
function makeNote() {
    const n = {id: Date.now(), t: "", c: ""}; // unclear
}
```

### Code Principles
- **Keep it Simple** - Dev Notes is intentionally a single file
- **No Dependencies** - Vanilla JavaScript only
- **Backward Compatible** - Don't break existing notes
- **Accessible** - Support keyboard navigation and screen readers
- **Performant** - Fast and responsive

## 📝 Commit Guidelines

Use clear, descriptive commit messages:

### Format
```
<type>: <subject>

<body>

<footer>
```

### Types
- **feat:** New feature
- **fix:** Bug fix
- **docs:** Documentation changes
- **style:** Code style changes (formatting, etc.)
- **refactor:** Code refactoring
- **test:** Adding tests
- **chore:** Maintenance tasks

### Examples
```bash
feat: add CSV export format for notes

Added ability to export notes as CSV in addition to JSON.
Includes note title, content, category, tags, and dates.

Closes #123
```

```bash
fix: prevent duplicate tags when adding quickly

Debounced tag input to prevent duplicates when user
presses Enter rapidly.
```

## 🚀 Pull Request Process

1. **Update Documentation**
   - Update README.md if needed
   - Add CHANGELOG.md entry
   - Include inline comments for complex code

2. **PR Title and Description**
   ```markdown
   Title: feat: add keyboard shortcut for quick search
   
   ## Description
   Adds Ctrl+K as alternative shortcut for search focus
   
   ## Changes
   - Added Ctrl+K handler in shortcuts system
   - Updated help modal with new shortcut
   - Added to README documentation
   
   ## Testing
   - [x] Tested on Chrome, Firefox, Safari
   - [x] Mobile responsive
   - [x] No console errors
   
   ## Screenshots
   [Include if UI changes]
   ```

3. **Review Process**
   - Maintainer will review within 48 hours
   - Address feedback promptly
   - Be patient and respectful

4. **After Merge**
   - Delete your feature branch
   - Pull latest changes to your fork
   - Celebrate your contribution! 🎉

## 💡 Feature Ideas

Looking for something to work on? Here are some ideas:

- **Enhanced Features**
  - Rich text editor toolbar
  - Note templates
  - Quick notes/scratch pad
  - Note linking/references
  - Full-text search with highlighting

- **Import/Export**
  - Markdown file import/export
  - Notion/Obsidian format support
  - Bulk operations

- **Organization**
  - Nested categories
  - Note archiving
  - Favorites/pinning
  - Sort options

- **Themes**
  - Additional color themes
  - Font size preferences
  - Custom CSS injection

## 🙏 Recognition

Contributors will be recognized in:
- README.md Contributors section
- Release notes
- Special thanks in documentation

## 📧 Questions?

Feel free to reach out:
- **Email:** edward.cox02@gmail.com
- **Issues:** Use GitHub issues for questions
- **Discussions:** Start a discussion thread

---

Thank you for contributing to Dev Notes! Every contribution, no matter how small, helps make Dev Notes better for everyone. 🚀
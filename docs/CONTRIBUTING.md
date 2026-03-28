# Contributing to AI Developer Learning Paths

Thank you for your interest in contributing to the AI Developer Learning Paths! This document provides guidelines and instructions for contributing.

## 🌟 Ways to Contribute

### 1. Report Issues
Found a bug, broken link, or outdated content? Please report it!

**Before submitting an issue:**
- Check if the issue already exists
- Provide a clear, descriptive title
- Include steps to reproduce (if applicable)
- Specify which track and week/day the issue affects

**Types of issues we track:**
- 🐛 Bugs (broken features, errors)
- 🔗 Broken links or resources
- 📝 Typos or grammar issues
- 📚 Outdated or incorrect content
- 💡 Feature requests
- ❓ Questions about content

### 2. Suggest Improvements
Have ideas for better explanations, new labs, or enhanced features?

**Good suggestions include:**
- Alternative explanations for complex topics
- Additional practice exercises
- New lab ideas with clear learning objectives
- UI/UX improvements
- Accessibility enhancements

### 3. Submit Pull Requests
Ready to contribute code or content? Follow these steps:

## 📋 Pull Request Process

### Step 1: Fork and Clone
```bash
# Fork the repository on GitHub, then clone your fork
git clone https://github.com/YOUR_USERNAME/ai-developer-learning-paths.git
cd ai-developer-learning-paths

# Add upstream remote
git remote add upstream https://github.com/dphadtare/ai-developer-learning-paths.git
```

### Step 2: Create a Branch
```bash
# Create a descriptive branch name
git checkout -b fix/broken-link-week2-day3
# or
git checkout -b feature/add-typescript-lab
# or
git checkout -b docs/improve-setup-guide
```

**Branch naming conventions:**
- `fix/` - Bug fixes, broken links, typos
- `feature/` - New labs, features, enhancements
- `docs/` - Documentation improvements
- `refactor/` - Code restructuring without changing functionality

### Step 3: Make Your Changes

**For content changes:**
- Edit the HTML files in `tracks/` directory
- Ensure formatting is consistent with existing content
- Test your changes locally by opening the HTML file in a browser
- Verify Chrome Gemini integration still works

**For documentation:**
- Edit markdown files in `docs/` or root directory
- Follow existing markdown formatting
- Keep language clear and concise

**For code/features:**
- Follow existing code style and patterns
- Test thoroughly in multiple browsers
- Ensure mobile responsiveness
- Don't break existing functionality

### Step 4: Test Your Changes

**Local testing checklist:**
- [ ] Open HTML files in Chrome, Firefox, and Safari
- [ ] Test on mobile devices or responsive mode
- [ ] Verify all links work
- [ ] Check Chrome Gemini integration (if applicable)
- [ ] Ensure progress tracking works
- [ ] Validate HTML (use W3C validator)
- [ ] Check for console errors

### Step 5: Commit Your Changes
```bash
# Stage your changes
git add .

# Commit with a clear message
git commit -m "Fix broken link in Week 2 Day 3 lab"
```

**Commit message guidelines:**
- Use present tense ("Add feature" not "Added feature")
- Be specific and descriptive
- Reference issue numbers if applicable (#123)
- Keep first line under 50 characters
- Add detailed description if needed

**Examples:**
```
Fix broken MDN link in JavaScript fundamentals (#45)

Add TypeScript migration lab to Week 6 Day 4

Improve setup guide with Windows-specific instructions

Refactor progress tracking to use sessionStorage
```

### Step 6: Push and Create PR
```bash
# Push to your fork
git push origin fix/broken-link-week2-day3

# Go to GitHub and create a Pull Request
```

**PR title and description:**
- Clear, descriptive title
- Explain what changed and why
- Reference related issues
- Include screenshots for UI changes
- List testing performed

**PR template:**
```markdown
## Description
Brief description of changes

## Type of Change
- [ ] Bug fix (non-breaking change fixing an issue)
- [ ] New feature (non-breaking change adding functionality)
- [ ] Breaking change (fix or feature causing existing functionality to change)
- [ ] Documentation update

## Related Issues
Fixes #123

## Testing
- Tested in Chrome, Firefox, Safari
- Verified on mobile (iOS/Android)
- Chrome Gemini integration works
- No console errors

## Screenshots (if applicable)
[Add screenshots here]

## Checklist
- [ ] My code follows the project's style
- [ ] I have tested my changes
- [ ] I have updated documentation (if needed)
- [ ] My changes don't break existing functionality
```

## 📝 Content Guidelines

### Writing Style
- **Clear and concise**: Avoid jargon, explain complex terms
- **Beginner-friendly**: Assume minimal prior knowledge
- **Practical**: Focus on real-world applications
- **Encouraging**: Use positive, supportive language
- **Inclusive**: Use gender-neutral language

### Code Examples
- Include comments explaining key concepts
- Use consistent formatting and indentation
- Provide complete, runnable examples
- Show both good and bad practices (when relevant)
- Include error handling

### Lab Structure
Each lab should include:
1. **Learning Objective**: What will students learn?
2. **Instructions**: Step-by-step guidance
3. **Code Examples**: Reference implementations
4. **Expected Output**: What success looks like
5. **Common Pitfalls**: What to watch out for
6. **Extension Challenges**: Optional advanced tasks

## 🎨 Design Guidelines

### HTML/CSS
- Use Tailwind CSS classes (already included via CDN)
- Maintain consistent spacing and typography
- Ensure mobile responsiveness (test at 320px, 768px, 1024px)
- Use semantic HTML elements
- Follow accessibility best practices (ARIA labels, alt text)

### Color Scheme
- **AI-Native Track**: Blue/Indigo gradient (#4f46e5, #3b82f6)
- **AI Agent Track**: Purple/Emerald gradient (#8b5cf6, #10b981)
- **Neutral**: Slate grays for text and backgrounds
- Maintain sufficient contrast (WCAG AA minimum)

### Typography
- Headings: Bold, clear hierarchy
- Body: 16px minimum for readability
- Code: Monospace font, distinct background
- Links: Underlined or clearly styled

## 🧪 Testing Requirements

### Browser Compatibility
Test in:
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

### Device Testing
- Desktop (1920x1080, 1366x768)
- Tablet (768x1024)
- Mobile (375x667, 414x896)

### Functionality Testing
- Navigation between weeks/days
- Lab expansion/collapse
- Progress tracking (localStorage)
- Chrome Gemini integration
- Copy-to-clipboard features
- Chart rendering (if applicable)

## 🚫 What Not to Do

- Don't add external dependencies without discussion
- Don't change the overall structure without approval
- Don't remove existing content without good reason
- Don't introduce breaking changes without warning
- Don't copy content from copyrighted sources
- Don't add tracking scripts or analytics without consent

## 📞 Getting Help

Stuck or have questions?

- **Questions**: Open a [GitHub Discussion](https://github.com/dphadtare/ai-developer-learning-paths/discussions)
- **Issues**: Check [existing issues](https://github.com/dphadtare/ai-developer-learning-paths/issues)
- **Clarifications**: Comment on the relevant issue or PR

## 🎯 Priority Areas

We especially welcome contributions in these areas:

1. **Accessibility improvements**: ARIA labels, keyboard navigation, screen reader support
2. **Mobile optimization**: Better responsive design, touch interactions
3. **Additional languages**: Translations to other languages
4. **More labs**: Especially advanced/challenging exercises
5. **Video tutorials**: Supplementary video content
6. **Community showcases**: Share your projects built using these paths

## 📜 Code of Conduct

### Our Standards

**Positive behavior includes:**
- Using welcoming and inclusive language
- Being respectful of differing viewpoints
- Gracefully accepting constructive criticism
- Focusing on what's best for the community
- Showing empathy towards others

**Unacceptable behavior includes:**
- Trolling, insulting/derogatory comments, personal attacks
- Public or private harassment
- Publishing others' private information
- Other conduct inappropriate in a professional setting

### Enforcement

Violations may result in:
1. Warning
2. Temporary ban from contributing
3. Permanent ban from the project

Report issues to: [Create a private issue or contact maintainer]

## 🏆 Recognition

Contributors will be:
- Listed in the project's contributors page
- Mentioned in release notes (for significant contributions)
- Credited in the acknowledgments section

## 📅 Review Process

- **Small fixes** (typos, broken links): Usually reviewed within 1-3 days
- **Content changes**: Reviewed within 1 week
- **New features**: May take 2-4 weeks for thorough review
- **Breaking changes**: Require discussion and approval from maintainers

## 🔄 Keeping Your Fork Updated

```bash
# Fetch upstream changes
git fetch upstream

# Merge upstream main into your branch
git checkout main
git merge upstream/main

# Push to your fork
git push origin main
```

---

Thank you for contributing to AI Developer Learning Paths! Your efforts help developers worldwide learn AI-powered development. 🚀

**Questions?** Open a [discussion](https://github.com/dphadtare/ai-developer-learning-paths/discussions) or comment on an existing issue.

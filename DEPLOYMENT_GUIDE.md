# Deployment Guide

This guide covers the remaining manual steps to complete the deployment of your AI Developer Learning Paths.

## ✅ Completed Steps

- [x] Repository created at `git@github.com:dphadtare/ai-developer-learning-paths.git`
- [x] All files committed and pushed to GitHub
- [x] Landing page with both learning tracks
- [x] Documentation (README, CONTRIBUTING, SETUP_GUIDE)
- [x] MIT License added
- [x] Open Graph meta tags for social sharing

## 🚀 Remaining Steps

### Step 1: Enable GitHub Pages (5 minutes)

1. Go to your repository: https://github.com/dphadtare/ai-developer-learning-paths

2. Click **Settings** (top navigation bar)

3. In the left sidebar, click **Pages**

4. Under **Source**:
   - Select: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/ (root)**
   - Click **Save**

5. Wait 2-5 minutes for deployment

6. Refresh the page - you'll see:
   ```
   Your site is live at https://dphadtare.github.io/ai-developer-learning-paths/
   ```

7. Click the URL to verify deployment

**Expected Result:** Your landing page should load with both learning tracks visible.

---

### Step 2: Configure Repository Settings (3 minutes)

#### A. Repository Description

1. Go to repository homepage: https://github.com/dphadtare/ai-developer-learning-paths

2. Click the ⚙️ (gear icon) next to "About" (top-right)

3. Fill in:
   - **Description**: `6-week AI developer learning paths with interactive labs and Chrome Gemini integration`
   - **Website**: `https://dphadtare.github.io/ai-developer-learning-paths/`
   - **Topics**: Add these tags (press Enter after each):
     - `ai`
     - `learning-path`
     - `education`
     - `javascript`
     - `ai-agents`
     - `mcp`
     - `prompt-engineering`
     - `tutorial`
     - `react`
     - `nodejs`
     - `python`
     - `langchain`

4. Check these boxes:
   - ☑️ **Releases** (for version tracking)
   - ☑️ **Packages** (if you add npm packages later)

5. Click **Save changes**

#### B. Enable Features

1. Still in **Settings**, scroll down to **Features**

2. Ensure these are checked:
   - ☑️ **Issues** (for bug reports and feature requests)
   - ☑️ **Discussions** (optional - for community Q&A)
   - ☑️ **Projects** (optional - for roadmap tracking)
   - ☑️ **Wiki** (optional - for additional docs)

3. Click **Save** if you made changes

#### C. Social Preview Image (Optional - can do later)

1. In **Settings**, scroll to **Social preview**

2. Click **Edit**

3. Upload an image (1280x640px recommended):
   - Create a banner with "AI Developer Learning Paths" text
   - Use gradient backgrounds matching your design
   - Include icons for both tracks

4. Or skip for now - GitHub will use default preview

---

### Step 3: Test Deployment (10 minutes)

#### A. Test Landing Page

Visit: https://dphadtare.github.io/ai-developer-learning-paths/

**Checklist:**
- [ ] Page loads without errors
- [ ] Both learning track cards are visible
- [ ] "Start JavaScript Track" button works
- [ ] "Start AI Agent Track" button works
- [ ] "View on GitHub" button works
- [ ] Footer links work
- [ ] Mobile responsive (test on phone or resize browser)

#### B. Test AI-Native Developer Track

Visit: https://dphadtare.github.io/ai-developer-learning-paths/tracks/ai-native-developer.html

**Checklist:**
- [ ] Page loads without errors
- [ ] Week tabs (W1-W6) are visible
- [ ] Day tabs (MON-FRI) work
- [ ] Labs expand/collapse correctly
- [ ] "Ask AI Mentor" buttons work (copy to clipboard)
- [ ] Progress tracking works (check/uncheck tasks)
- [ ] Charts render correctly
- [ ] Mobile responsive

#### C. Test AI Agent Developer Track

Visit: https://dphadtare.github.io/ai-developer-learning-paths/tracks/ai-agent-developer.html

**Checklist:**
- [ ] Page loads without errors
- [ ] Week tabs (W1-W6) are visible
- [ ] Day tabs (MON-FRI) work
- [ ] Labs expand/collapse correctly
- [ ] "Ask AI Mentor" buttons work (copy to clipboard)
- [ ] Progress tracking works (check/uncheck tasks)
- [ ] Charts render correctly
- [ ] Mobile responsive

#### D. Test Chrome Gemini Integration

1. Open any track page
2. Click an "Ask AI Mentor" button
3. Verify:
   - [ ] Toast notification appears
   - [ ] Prompt is copied to clipboard
   - [ ] Press Ctrl+Shift+. (or ⌘+Shift+. on Mac)
   - [ ] Gemini sidebar opens
   - [ ] Paste works (Ctrl+V or ⌘+V)
   - [ ] Gemini responds with relevant help

#### E. Test on Multiple Browsers

Test on:
- [ ] Chrome (latest)
- [ ] Firefox (latest)
- [ ] Safari (latest) - if on Mac
- [ ] Edge (latest) - if on Windows

#### F. Test Mobile Responsiveness

Test on actual devices or browser dev tools:
- [ ] iPhone (375x667, 414x896)
- [ ] Android (360x640, 412x915)
- [ ] Tablet (768x1024)

**Common issues to check:**
- Text is readable (not too small)
- Buttons are tappable (not too small)
- No horizontal scrolling
- Navigation works on touch
- Charts fit on screen

---

### Step 4: Create Issue Templates (Optional - 5 minutes)

1. In your repository, go to **Settings** → **Features**

2. Scroll to **Issues**

3. Click **Set up templates**

4. Add these templates:
   - **Bug report** (for broken features)
   - **Feature request** (for new ideas)
   - **Question** (for help requests)

5. Customize and commit

---

### Step 5: Add GitHub Actions (Optional - for automation)

Create `.github/workflows/test-links.yml`:

```yaml
name: Test Links

on:
  push:
    branches: [ main ]
  pull_request:
    branches: [ main ]
  schedule:
    - cron: '0 0 * * 0'  # Weekly on Sunday

jobs:
  test-links:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - name: Check links
        uses: gaurav-nelson/github-action-markdown-link-check@v1
        with:
          use-quiet-mode: 'yes'
```

This will automatically check for broken links weekly.

---

### Step 6: Promote Your Learning Paths (Ongoing)

#### A. Share on Social Media

**Twitter/X:**
```
🚀 Just launched: AI Developer Learning Paths!

Two comprehensive 6-week programs:
💻 AI-Native Developer (JavaScript, React, APIs)
🤖 AI Agent Developer (MCP, Prompt Engineering)

✨ Interactive labs
📊 Progress tracking
🧠 Chrome Gemini AI mentor

Free & open source!

https://dphadtare.github.io/ai-developer-learning-paths/

#AI #Learning #JavaScript #Agents
```

**LinkedIn:**
```
I'm excited to share the AI Developer Learning Paths - two comprehensive, free learning programs I've created for developers looking to master AI-powered development.

🎯 What's included:
• 6-week structured curriculum for each track
• 60+ hands-on labs with real-world scenarios
• Built-in Chrome Gemini AI mentor integration
• Progress tracking and self-paced learning

💻 AI-Native Developer Track:
Master full-stack development with JavaScript, Node.js, React, PostgreSQL, and production deployment.

🤖 AI Agent Developer Track:
Build intelligent AI systems with prompt engineering, MCP, tool development, and agent orchestration.

Both tracks are completely free and open source. Check them out:
https://dphadtare.github.io/ai-developer-learning-paths/

I'd love to hear your feedback and contributions!

#AILearning #WebDevelopment #AIAgents #OpenSource
```

**Reddit:**
- r/learnprogramming
- r/webdev
- r/javascript
- r/reactjs
- r/MachineLearning
- r/artificial

#### B. Submit to Awesome Lists

Search for and submit to:
- awesome-learning-resources
- awesome-ai
- awesome-javascript
- awesome-react
- awesome-nodejs

#### C. Share on Dev Communities

- Dev.to
- Hashnode
- Medium
- Hacker News (Show HN)
- Product Hunt

#### D. Add to Your Profile

Update your GitHub profile README to showcase this project.

---

## 🎉 Success Checklist

Before considering deployment complete:

- [ ] GitHub Pages is live and accessible
- [ ] Repository description and topics are set
- [ ] Issues and Discussions are enabled
- [ ] Landing page works on all browsers
- [ ] Both learning tracks load correctly
- [ ] Chrome Gemini integration works
- [ ] Mobile responsive on all pages
- [ ] All links work (no 404s)
- [ ] Progress tracking persists
- [ ] Charts render correctly

---

## 📊 Monitoring

### Track Success Metrics

Check these regularly in GitHub Insights:

1. **Traffic** (Settings → Insights → Traffic)
   - Unique visitors
   - Page views
   - Referring sites

2. **Engagement** (Settings → Insights)
   - Stars
   - Forks
   - Issues opened
   - Pull requests

3. **Community** (Settings → Insights → Community)
   - Contributors
   - Discussions
   - Issue response time

### Set Goals

Example goals:
- 100 stars in first month
- 10 contributors in first quarter
- 1000 unique visitors per month
- 5 community discussions per week

---

## 🐛 Troubleshooting

### GitHub Pages not deploying

**Solution:**
1. Check Settings → Pages for error messages
2. Ensure `index.html` exists in root
3. Wait 5-10 minutes (initial deployment can be slow)
4. Check GitHub Actions tab for build errors

### 404 errors on track pages

**Solution:**
1. Verify files exist in `tracks/` directory
2. Check file names match links exactly (case-sensitive)
3. Clear browser cache
4. Wait for GitHub Pages to rebuild

### Charts not rendering

**Solution:**
1. Check browser console for errors
2. Verify Chart.js CDN is accessible
3. Test in different browser
4. Check if JavaScript is enabled

### Chrome Gemini not working

**Solution:**
1. Verify Chrome is up to date
2. Check if Gemini is available in user's region
3. Test clipboard API (requires HTTPS)
4. Provide fallback instructions in SETUP_GUIDE.md

---

## 📞 Need Help?

If you encounter issues during deployment:

1. Check GitHub Pages documentation: https://docs.github.com/en/pages
2. Open an issue in your repository
3. Ask in GitHub Discussions
4. Check browser console for errors

---

## ✅ Next Steps After Deployment

1. **Monitor analytics** - Track visitor engagement
2. **Respond to issues** - Help users who encounter problems
3. **Accept contributions** - Review and merge PRs
4. **Update content** - Keep labs current with latest tech
5. **Add features** - Consider adding:
   - Certificate of completion
   - User accounts (optional)
   - Community showcase
   - Video tutorials
   - Downloadable resources

---

**Congratulations!** 🎉 Your AI Developer Learning Paths are now live and ready to help developers worldwide!

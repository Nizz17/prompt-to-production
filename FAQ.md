# Frequently Asked Questions (FAQ) 💡

## 🛠 Git & GitHub Issues

### When should I open an Issue?
- **Bug Reports:** If you find something broken in the starter code.
- **Clarification:** If the instructions for a User Case (UC) are confusing.
- **Stuck:** If you've been debugging for more than 5 minutes and need help from a tutor (mention them with @username).

### How do I open a good Issue?
1. Click the **Issues** tab -> **New Issue**.
2. Give it a clear title (e.g., `[UC-0A] Confusion about severity keywords`).
3. Describe what you're seeing and what you expected.
4. Add a screenshot if it helps!

---

## 🚀 Creating a Pull Request (PR)

### Step 1: Fork the Repo
Click the **Fork** button at the top right of this page. This creates a copy of the workshop code in your own GitHub account.

### Step 2: Clone Your Fork
Copy your fork's URL and run:
```bash
git clone https://github.com/[your-username]/prompt-to-production.git
cd prompt-to-production
```

### Step 3: Create a Branch
**Crucial:** Do not work on the `main` branch. Create a new one:
```bash
git checkout -b participant/[your-name]-[city]
# Example: git checkout -b participant/arshdeep-pune
```

### Step 4: Commit & Push
Follow the commit message standard mentioned in the README:
```bash
git add .
git commit -m "[UC-0A] Fix severity: missing keywords → added triggers"
git push origin participant/[your-name]-[city]
```

### Step 5: Open the PR
1. Go to the **original** repository (nasscomAI/prompt-to-production).
2. You'll see a yellow bar saying "Compare & pull request" — click it!
3. Ensure the **base** is `nasscomAI/main` and the **head** is your branch.
4. Fill out the PR template completely.

---

## 🚧 Common Troubleshooting

### My PR has a red 'X' (Validation Failed)
Check the **Actions** tab. It's likely one of two things:
1. **Commit Message:** Ensure your message follows the exact `[UC-ID] Fix... → ...` format.
2. **Python Syntax:** Your script might have a typo. Run it locally first!

### How do I sync my fork with the main repo?
If the workshop leads update the main repo, you can sync yours by clicking **Sync fork** on your GitHub repo page or running:
```bash
git fetch upstream
git merge upstream/main
```

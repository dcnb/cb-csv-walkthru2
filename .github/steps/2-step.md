## Step 2: Sign Your Work with Git

Great work! Your Codespace is ready. Now let's learn the **Git workflow** by making your first meaningful commit. You'll add your name to the site configuration—a fundamental skill you'll use throughout this tutorial.

### 📖 Theory: Understanding the Git Workflow

**Git** is a version control system that tracks changes to your files. Every change you make goes through three stages:

1. **Edit** - Modify files in your editor
2. **Stage** (`git add`) - Mark which changes you want to save
3. **Commit** (`git commit`) - Save a snapshot with a descriptive message
4. **Push** (`git push`) - Upload your commits to GitHub

Think of it like packing a box:
- **Edit** = Put items on the table
- **Stage** = Put specific items in the box
- **Commit** = Seal the box with a label
- **Push** = Ship the box to storage

> [!IMPORTANT]
> Always write clear commit messages! They help you (and others) understand what changed and why.

### ⌨️ Activity: Add Your Name as Author

Let's personalize the site by adding your name to the configuration file.

1. In the Codespace **file explorer** (left sidebar), click to open `_config.yml`
1. Find line 30 that says `author: CollectionBuilder`
1. Change it to `author: Your Name` (use your actual name!)
1. **Save the file** by pressing `Ctrl+S` (Windows/Linux) or `Cmd+S` (Mac)
   - Or go to **File → Save** in the menu

> [!NOTE]
> The `_config.yml` file contains site-wide settings for your CollectionBuilder site. Jekyll (the static site generator) reads this file to configure your collection.

1. In the **terminal** at the bottom, run these Git commands:

```bash
git add _config.yml
git commit -m "Add my name as author"
git push
```

**What just happened?**
- `git add _config.yml` - Staged your change
- `git commit -m "..."` - Created a snapshot with a message
- `git push` - Uploaded your commit to GitHub

Wait for Mona to check your work! 🤖

<details>
<summary>Having trouble? 🤷</summary><br/>

- Make sure you **saved the file** (`Ctrl+S` or `Cmd+S`) before running Git commands
- Check that the terminal shows no errors after each command
- If `git push` asks for credentials, the Codespace should handle authentication automatically
- You can verify your change was saved by looking at the file—unsaved files show a dot (•) next to their name

</details>

## Step 1: Launch Your Development Environment

Digital collections need a development environment to build and preview before publishing. You'll use **GitHub Codespaces**, which gives you a full Visual Studio Code editor and terminal running in your browser—no installation required!

### 📖 Theory: What is GitHub Codespaces?

GitHub Codespaces is a cloud-based development environment that runs Visual Studio Code in your browser. When you launch a Codespace, GitHub creates a virtual machine with:

- **File explorer** (left sidebar) - browse and open files
- **Editor** (center) - edit code and text files
- **Terminal** (bottom) - run commands like Git, Jekyll, and bundle
- **Extensions** - tools that enhance the editor

Codespaces are perfect for tutorials because they provide a consistent environment—everyone gets the same setup, regardless of their operating system.

> [!TIP]
> Codespaces are free for personal GitHub accounts with 120 core-hours per month and 15 GB storage.

### ⌨️ Activity: Open GitHub Codespace

Let's launch your development environment!

1. Click the **Code** button (green button at the top of this repository)
1. Click the **Codespaces** tab
1. Click **Create codespace on main**
1. Wait for the Codespace to load (this may take 1-2 minutes)

Once your Codespace opens, you'll see VS Code running in your browser with:
- A file explorer on the left showing your repository files
- A terminal at the bottom (if not visible, go to **Terminal → New Terminal**)

> [!NOTE]
> The terminal is where you'll run Git commands, preview your site, and more. Think of it as a command-line interface to your project.

1. In the terminal at the bottom, run this command to create a marker file:

```bash
echo "Codespace initialized" > .codespace-ready
git add .codespace-ready
git commit -m "Initialize Codespace"
git push
```

Wait for Mona to check your work! 🤖

<details>
<summary>Having trouble? 🤷</summary><br/>

- Make sure you clicked "Create codespace on **main**" (not a different branch)
- If the terminal isn't visible, go to **Terminal → New Terminal** in the menu
- Copy and paste the commands one by one, pressing Enter after each
- If you get an error about Git configuration, that's normal—the push command will still work

</details>

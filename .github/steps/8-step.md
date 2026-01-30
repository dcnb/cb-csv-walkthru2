## Step 8: Publish to GitHub Pages

You've built an amazing digital collection! Now let's publish it to the web with **GitHub Pages** so anyone can visit your collection.

### 📖 Theory: GitHub Pages and Static Site Deployment

**GitHub Pages** is a free hosting service from GitHub that publishes static websites directly from your repository. When you push commits, GitHub Actions automatically:

1. Runs Jekyll to build your site
2. Generates HTML, CSS, and JavaScript files
3. Deploys them to a public URL

Your collection will be available at: `https://[username].github.io/[repository-name]`

CollectionBuilder sites are **static**, meaning:
- No database required
- Fast loading
- Free hosting on GitHub Pages
- Easy to preserve and maintain

> [!TIP]
> GitHub Pages is free for public repositories. Your collection will be accessible to anyone on the internet!

### ⌨️ Activity: Configure and Deploy Your Site

Let's set up GitHub Pages and configure your site for production.

1. Go to your repository on GitHub (click the repository name at the top)
1. Click **Settings** (top right)
1. In the left sidebar, click **Pages**
1. Under "Build and deployment", set **Source** to **GitHub Actions**
   - This tells GitHub to use the Jekyll workflow included with CollectionBuilder

> [!NOTE]
> CollectionBuilder includes a `.github/workflows/jekyll.yml` file that automatically builds and deploys your site when you push to the main branch.

1. Now, back in your Codespace, open `_config.yml` one more time

1. Update these deployment settings with **your** GitHub username and repository name:

   - Line 11: `url: https://[username].github.io`
   - Line 13: `baseurl: /[repository-name]`
   - Line 15: `source-code: https://github.com/[username]/[repository-name]`

   **Example** (if your username is `octocat` and your repo is `my-psychiana-collection`):
   ```yaml
   url: https://octocat.github.io
   baseurl: /my-psychiana-collection
   source-code: https://github.com/octocat/my-psychiana-collection
   ```

> [!IMPORTANT]
> The `baseurl` must start with `/` and match your repository name exactly. The `url` should NOT include the repository name.

1. **Save the file** (`Ctrl+S` or `Cmd+S`)

1. Commit and push your changes:

```bash
git add _config.yml
git commit -m "Configure for GitHub Pages deployment"
git push
```

1. Go to the **Actions** tab in your repository on GitHub
1. Watch the workflow run (it will take 2-5 minutes)
1. Once it shows a green checkmark ✅, visit your live site at:
   ```
   https://[username].github.io/[repository-name]
   ```

🎉 **Congratulations!** Your digital collection is now live on the web!

Share your published collection URL below! 🌐

<details>
<summary>Having trouble? 🤷</summary><br/>

- Make sure the `url` and `baseurl` match your GitHub username and repository name exactly
- The `baseurl` should start with `/` (e.g., `/my-repo`, not `my-repo`)
- If the Actions workflow fails, click on it to see error details
- It can take a few minutes after the green checkmark for the site to be fully live
- If you see 404 errors, double-check your `baseurl` setting

</details>

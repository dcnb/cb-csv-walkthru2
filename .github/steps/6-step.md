## Step 6: Preview Your Collection Locally

Excellent! Your site is configured. Now for the exciting part—let's **build and preview** your collection in the browser!

### 📖 Theory: Jekyll, Ruby, and Bundle

CollectionBuilder uses several technologies to build your site:

- **Ruby** - A programming language
- **Bundler** (`bundle`) - A Ruby tool that manages dependencies (libraries your project needs)
- **Jekyll** - A static site generator (written in Ruby) that builds HTML from your metadata and templates

The workflow is:
1. `bundle install` - Install all dependencies (you only do this once, or when dependencies change)
2. `bundle exec jekyll serve` - Build your site and start a local web server
3. Open the preview in your browser

> [!TIP]
> The `jekyll serve` command watches for file changes and automatically rebuilds your site. Leave it running while you work!

### ⌨️ Activity: Build and Preview Your Collection

Let's see your Psychiana collection come to life!

1. In the Codespace terminal, run:

```bash
bundle install
```

This installs all the Ruby gems (libraries) your site needs. It may take 1-2 minutes. You'll see lots of output—that's normal!

> [!NOTE]
> You only need to run `bundle install` once (or when dependencies change). Don't worry if you see warnings—as long as it says "Bundle complete!" at the end, you're good.

1. Once `bundle install` finishes, run:

```bash
bundle exec jekyll serve
```

This builds your site and starts a local web server. You'll see output ending with something like:

```
Server address: http://127.0.0.1:4000
Server running... press ctrl-c to stop.
```

1. Look for a **pop-up notification** in the bottom-right that says "Open in Browser" and **click it**
   - If you miss it, click the **PORTS** tab (next to TERMINAL) and click the globe icon 🌐 next to port 4000

1. **Explore your collection!** Check out:
   - The home page
   - The Browse page (all items)
   - The Map page (items with coordinates)
   - The Timeline page
   - Click on an item to see its detail page

> [!IMPORTANT]
> Leave the Jekyll server running! Go back to the terminal and press `Ctrl+C` only when you're done previewing.

When you're ready to continue, press `Ctrl+C` in the terminal to stop the server, then push a marker commit:

```bash
echo "Previewed collection locally" > .preview-complete
git add .preview-complete
git commit -m "Complete local preview"
git push
```

Wait for Mona to check your work! 🤖

<details>
<summary>Having trouble? 🤷</summary><br/>

- If `bundle install` fails, try running it again—sometimes downloads time out
- If port 4000 is already in use, Jekyll will try port 4001, 4002, etc.
- If you don't see the pop-up, manually click the PORTS tab and click the globe icon
- If you see errors about missing files, make sure you completed Step 5 correctly
- To stop Jekyll, press `Ctrl+C` in the terminal (not `Cmd+C`)

</details>

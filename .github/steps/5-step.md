## Step 5: Configure Your Site for Psychiana

Great! You've edited metadata. Now let's configure the site to actually **use** the Psychiana collection. This is a critical step—without it, your site won't know which CSV file to read!

### 📖 Theory: Jekyll Configuration and the _config.yml File

**Jekyll** is a static site generator that transforms your metadata and templates into a complete website. It reads `_config.yml` to understand:

- **Site settings**: Title, tagline, description
- **Collection settings**: Which metadata CSV to use
- **Deployment settings**: URL and baseurl for publishing

The most important setting for CollectionBuilder is the `metadata:` field. This tells Jekyll which CSV file in `_data/` contains your collection data.

> [!IMPORTANT]
> After changing `_config.yml`, you must restart Jekyll for changes to take effect (we'll do this in the next step).

### ⌨️ Activity: Point Your Site to the Psychiana CSV

Currently, your site is configured to use demo metadata. Let's change it to use the Psychiana collection.

1. In your Codespace, open `_config.yml`
1. Find line 37, which says: `metadata: demo-compoundobjects-metadata`
1. Change it to: `metadata: psychiana`

   **Before:**
   ```yaml
   metadata: demo-compoundobjects-metadata
   ```

   **After:**
   ```yaml
   metadata: psychiana
   ```

> [!NOTE]
> Notice we write `psychiana`, not `psychiana.csv`—Jekyll automatically looks in the `_data/` folder and adds the `.csv` extension.

1. While you're here, let's also update the site title and description. Change these lines:
   - Line 21: `title: Psychiana Digital Collection`
   - Line 23: `tagline: A Mail-Order Religion from Moscow, Idaho`
   - Line 26: `description: "The Psychiana Digital Collection documents Frank B. Robinson's mail-order religion (1928-1948)."`

1. **Save the file** (`Ctrl+S` or `Cmd+S`)

Now commit your changes:

```bash
git add _config.yml
git commit -m "Configure site for Psychiana collection"
git push
```

Wait for Mona to check your work! 🤖

<details>
<summary>Having trouble? 🤷</summary><br/>

- The `metadata:` field is in the "COLLECTION SETTINGS" section of `_config.yml`
- Make sure you write `metadata: psychiana` exactly (no quotes, no `.csv`)
- YAML is picky about spacing—keep the same indentation
- Don't forget to save before committing!

</details>

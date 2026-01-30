## Step 4: Edit Collection Metadata

Now that you understand the CSV structure, let's make a change! You'll edit metadata and commit it using the Git workflow you learned in Step 2.

### 📖 Theory: Why Metadata Matters

Metadata is the foundation of your digital collection. When you change metadata:

- **Item pages update** - Titles, descriptions, and details change
- **Search results change** - Updated text becomes searchable
- **Maps recalculate** - If you edit latitude/longitude
- **Timelines adjust** - If you edit dates

CollectionBuilder is **metadata-driven**, meaning the CSV controls everything. Change the data, change the site!

> [!IMPORTANT]
> Always keep your `objectid` values unique and consistent. They're used to link metadata to digital files and generate item URLs.

### ⌨️ Activity: Customize an Item

Let's personalize item `psychiana001` by changing its title.

1. In your Codespace, open `_data/psychiana.csv` (if not already open)
1. Find the row for `psychiana001` (should be the first data row after the header)
1. Locate the `title` column
1. Change the title to something creative! For example:
   - Original: `Frank Robinson and his electric machine`
   - Your version: `Frank Robinson's Revolutionary Electric Machine` (or your own creative title!)
1. **Save the file** (`Ctrl+S` or `Cmd+S`)

Now commit your change using the Git workflow:

```bash
git add _data/psychiana.csv
git commit -m "Update metadata for psychiana001"
git push
```

> [!NOTE]
> When editing CSV files in text editors, be careful not to accidentally delete commas or quotation marks—they're part of the file structure!

Wait for Mona to check your work! 🤖

<details>
<summary>Having trouble? 🤷</summary><br/>

- Make sure you're editing `_data/psychiana.csv`, not a different CSV file
- The title field should be easy to spot—it's one of the first columns
- If the CSV looks confusing, try opening it in a spreadsheet program, editing there, and saving
- Remember to **save the file** before running Git commands
- If you make a mistake, you can undo (`Ctrl+Z` or `Cmd+Z`) before saving

</details>

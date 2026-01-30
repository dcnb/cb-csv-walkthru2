## Step 3: Explore Collection Metadata

Excellent! You've made your first commit. Now let's explore the heart of CollectionBuilder: the **metadata CSV file** that describes your digital collection.

### 📖 Theory: Metadata and CSV Files

**Metadata** means "data about data"—it's information that describes your collection items. For a digital collection, metadata includes:

- **Descriptive info**: Title, description, creator, date
- **Technical info**: Format, file location, file size
- **Administrative info**: Rights, subjects, keywords
- **Geospatial info**: Latitude, longitude (for maps!)

**CSV (Comma-Separated Values)** is a simple format for tabular data:
- Each row represents one collection item
- Each column represents one metadata field
- The first row contains column headers

CollectionBuilder reads your CSV and transforms it into:
- 📖 Item pages
- 🗺️ Interactive maps (using latitude/longitude)
- 📅 Timelines (using dates)
- 🔍 Search functionality
- 📊 Data visualizations

> [!TIP]
> CSV files can be edited in spreadsheet programs (Excel, Google Sheets) or text editors. For this tutorial, we'll edit in VS Code to practice file-based workflows.

### ⌨️ Activity: Explore the Psychiana Metadata

Let's examine the metadata structure for the Psychiana collection.

1. In the Codespace file explorer, navigate to `_data/psychiana.csv`
1. Click to open the file

You'll see columns like:
- `objectid` - Unique identifier for each item
- `title` - Item title
- `description` - Item description
- `format` - Media type (Image, Sound, etc.)
- `latitude` and `longitude` - Geographic coordinates
- `date` - Creation date

1. **Count the different formats**: Scroll through and note how many different `format` types you see (Image, Sound, etc.)
1. **Find geographic items**: Look for items with `latitude` and `longitude` values—these will appear on the map!

> [!NOTE]
> Notice item `psychiana001`? We'll edit that in the next step. For now, just explore and get familiar with the structure.

That's it for this step—just exploration! Click below when you're ready to continue.

Ready to move on? I'll continue watching for your next commit! 🤖

<details>
<summary>Having trouble? 🤷</summary><br/>

- The CSV file is located at `_data/psychiana.csv` in the file explorer
- You don't need to edit anything in this step—just explore!
- CSV files look best in spreadsheet programs, but VS Code works fine for viewing
- Don't worry if the file looks messy—that's normal for CSVs in text editors

</details>

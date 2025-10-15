# Build your MOREL website from a Zotero collection in 7 simple steps
- **Prepare the Zotero Fields** for a MOREL website {#zotero-fields}. MOREL items are added in the same way that items are added in any [Zotero library](https://www.zotero.org/support/adding_items_to_zotero). In its current version, MOREL can only process items of type `book`. Since not all the fields needed for MOREL are available for the `book` content type, some considerations must be made:
    - Excerpt: the fragment from each MOREL record corresponds to the `notes` of Zotero (see the [documentation](https://www.zotero.org/support/notes) about Zotero notes). In its current version, MOREL *only accepts one excerpt per book*.
    - Cover: the cover is a jpg file that is added as an `attachment` to the Zotero item (see the Zotero attachments [documentation](https://www.zotero.org/support/attaching_files)).
- **Fork this repository** — that is, create a copy in your [GitHub](https://github.com) account.
- **Go to the `actions` tab** and enable workflows.
- **Open `_config.yml` and change**:
  - The `title` to your site's.
  - The `tagline` to your site's.
  - The `email` and/or social media accounts to your site's.
  - The `jotform` link (create your free account at https://www.jotform.com/).
- **Go to the `settings` tab**, open the `pages` section, and select `gh-pages` as the branch that will build the site.
- **Open the file `_abouts/site-description.md`** and write a description for your site. The `<!-- more -->` line separates what appears in the footer across all pages from the longer description that appears on the `about` page only.
- **Generate the content from Zotero** by exporting a collection, subcollection or library as a `csv` file, and replacing the content of `assets/data/books_zotero.csv`



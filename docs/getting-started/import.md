---
title: Import Data
slug: /import
---
Raindrop.io supports importing bookmarks from web browsers and services in [various formats](#supported-formats). 

## How to import?
1. Grab export file. Check [supported formats](#supported-formats) and [limitations](#limitations) below
2. Upload this file [**here**](https://app.raindrop.io/settings/import)
3. Fine tune [import settings](#settings) (optional)
4. Click **Start import** and wait for upload is complete

:::note
* Do not close browser tab until upload is complete
* Bookmark thumbnails and search filters will be fetched shortly after import is complete. You will receive an email notification.
:::

## Supported Formats
### Netscape HTML
Almost any service or browser can generate this file for you. Here how to get it from popular browsers and services:
[Chrome](https://www.wikihow.com/Export-Bookmarks-from-Chrome),
[Safari](https://www.ionos.com/digitalguide/websites/web-development/export-safari-bookmarks/),
[Firefox](https://support.mozilla.org/en-US/kb/export-firefox-bookmarks-to-backup-or-transfer),
[Pocket](https://help.getpocket.com/article/1015-exporting-your-pocket-list),
[Google Bookmarks](https://www.google.com/bookmarks#:~:text=export%20bookmarks)

### CSV
We support almost any `CSV` file generated by third-party bookmarking apps.

<!------------------------------>
<details><summary>

#### How to prepare my own CSV file?

</summary>

If you want to upload your own CSV file just make sure:

- Comma delimited
- Columns: `url`, `folder`, `title`, `description`, `tags`, `created`
- `url` column is required, other are optional
- use `/` to specify nested `folder`, like `a/b/c`
- to have multiple `tags` just put them in quotes, like `"tag1, tag2"`
- `created` column should have Unix timestamp or date in ISO 8601 format
- Column order doesn't matter

Here an example CSV file:
```csv
folder,url,title,description,tags,created
"Folder",http://google.com,Google,"Search engine","search, app",1629980125
"Folder/Nested folder",http://yahoo.com,Yahoo,"Another search engine","search, app",1629980125
```

[Validate your CSV](https://csvlint.io/) file before uploading!
</details>

### TXT
Txt file should have a url per row

### ENEX (Evernote)
You can transfer all your web-clips (bookmarks) from Evernote to Raindrop.io, description and tags will be imported as well.
Be sure to select `ENEX` as a file format of [export in Evernote](https://help.evernote.com/hc/en-us/articles/209005557-Export-notes-and-notebooks).

### Pinterest
Pinterest itself doesn't have any tools to export your data. But you can try to use great third-party app called [Pinback](https://pinbackit.github.io/) that can help you download export file.
Just follow instructions on [Pinback](https://pinbackit.github.io/) site.

## Settings
Before you start import, please select how much data you want to transfer:

Mode | Description
---- | -----------
**Only new folders and bookmarks** | When you upload the same import file again but with new data, this mode will prevent uploading duplicates and ensure structure untouched, only new folders and bookmarks will be imported. <br/><br/> If you not sure select this mode
**Import all** | Select this mode if you want to import everything as is (including duplicates)
**Start from scratch** | This mode is the best way to clean your account data completely and replace it with data from import file. <br/> Be sure if you already have any data in Raindrop it will be removed and replaced.

## Limitations
- We support files up to 50Mb in size. If you have a larger file just archive it (as ZIP file)
- Evernote attachments are not supported yet
- Google Bookmarks file should have a `GoogleBookmarks.html` file name to properly import it
---
title: Web, Desktop App & Extension
slug: /changelog
---

### 5.4.5
- Remove Google Analytics
- No more ask for save unsaved changes when you just navigate to other screen inside of an app
- When you press `Tab` in tags field, highlighted tag will be selected instead of creating new one
- Remove auto-close from add bookmark window
- Fix add bookmark window in Brave browser
- Fix Safari extension in-app purchase window when you click on any link

### 5.4.2
- Search
    - Now 5x time faster
    - New [advanced search operators](../using/search/index.md#operators)
        - Find exact phrase
        - Exclude conditions
        - Match any condition
        - Search for items created/updated in specific date
        - Find by any part of an URL
        - Find items that have (or not) a permanent copy
        - Find only in title/description (turn off full-text search)
    - Now it's possible to search by a part of a word
    - [Recent searches](../using/search/index.md#recent)
- Extension
    - New overlay save page/link dialog (when you save by hotkey or a context menu)
        - Now it opened inline on a page unlike old window that you need manually close all the time
        - It automatically closes after a few seconds
    - Cover selector now shows 10 images from web-page
    - Significantly improve initial load time of a extension popover
    - Significantly improved parser (especially for Youtube)
    - Safari specific
        - Fix annoing permissions dialog
        - Show [✔] as badge
        - Fix hotkeys visibility in settings
        - Hide omnibox option (not available in Safari)
- Overall
    - New settings page design
    - New sepia theme
    - Improve translation for almost all languages

### 5.4.0
- Save all tabs
    - Click `Tabs...` in bottom right corner if you have `Clipper` extension mode
    - Mouse over `Save` button and click `Save tabs` if you have `Mini App` extension mode

### 5.3.34
- New Share window
    - Now you can add description and embed to website/blog
- New [Remove all empty collections](../using/collections/index.md#remove-all-empty) action
- Fix tags autocomplete, do not submit form when some tag is highlighted
- Fix bug when all new tags are lowercase by default
- Fix gap between bookmarks buttons in Safari
- Fix Maximum call stack size exceeded error for some users
- Fix search bug when query have a percent symbol
- Improve translation

### 5.3.31
- Improve search
- If you don't like default sorting `by relevance` for search you can change it now in [settings](https://app.raindrop.io/settings/app)

### 5.3.30
- Now you can upload your own avatar in [settings](https://app.raindrop.io/settings/account)
- Login or register with username
- Now everywhere in the app `username` is showed instead of a real name
    - You can change your `username` in [settings](https://app.raindrop.io/settings/account)
    - Why? To improve privacy (1), new public pages will have `username` in URL's (2) and it's just convinient to login with a username instead of email (3)

### 5.3.25
- Tags autocomplete now shows a new tag as separate item (more obvious how to create a new tag)

### 5.3.24
- Speed up saving new bookmarks speed in extension (nearly instant now)
- Unsaved changes warning bug fix
- Improve translation ES, IT, PL
- Sort search results by relevancy by default
- Improve compatibility with old browsers (Chrome >= 67, Safari >= 10, Firefox >= 55, Edge >= 80)
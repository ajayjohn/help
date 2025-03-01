---
title: Public Page
slug: /public-page
---

Your bookmarks and collections are private by default, but with one click, you can generate a public link to share them with entire web.
Anyone with the link (sign-up is not required) will be able to view your wall but not edit it.

![](page.jpg)

:::note
[Read this article](../collaboration/index.md) if you want to give an edit access to your collection.
:::

## Enable Public Page

1. Go to [web app](https://app.raindrop.io/)
2. Open the collection you want to share, then click the `Share` button in top right corner of the screen.

![](share.png)

3. From here just turn on `Public Page` and copy URL

<p><img src={require('./bylink.png').default} height='496' /></p>

:::note
If you need to embed bookmarks to your website or blog read [this article](../embed/index.md)
:::

## Customize
You can change appearance of your public page by appending special parameters at the end of a URL.

Imagine you have such public page URL: `https://raindrop.io/exentrich/design-66`, just add `/view/...parameters-here...` at the end, so final URL will be for example `https://raindrop.io/exentrich/design-66/view/theme=dark&sort=-title&page=3`

Notice that parameter and value is divided by `=`, and there `&` between each parameter-value group.

Parameter | Possible values | Default value | Description
--- | --- | --- | ---
`sort` | `-created`, `created`, `-title`, `title` | `-created` | Bookmarks order
`search` | `#tag` or `apple`, etc... | none | Search query
`theme` | `light`, `dark` or `auto` | `light` | Theme
`page` | `0`, `1`, `2`, etc... | `0` | Pagination
`perpage` | `1`, `2`, ... max `50` | `30` | How many bookmarks per page
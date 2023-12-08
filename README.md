# `<share-controls>` element
A Custom Element that adds progressively enhanced share buttons to your web page. This custom element was inspired by this [excellent article](https://set.studio/simplify-sharing-with-built-in-apis-and-progressive-enhancement/) on the [Set Studio](https://set.studio/) blog.

## Usage
Add the `<share-controls>` element to your page and provide a simple fallback.

```html
<share-controls>
  <p>Copy and paste to share this article: {{ Your URL here }}
</share-controls>
```

By default the URL that gets copied to the clipboard and/or shared via the native web share API is the current page URL, but you can also use the provided `url` attribute to specify a different URL if you need to.

```html
<share-controls url="https://levimcg.com/blog/">
  <p>Copy and paste to share this article: {{ Your URL here }}
</share-controls>
```

## Attributes

| Attribute      | Description                                                                   |
| -------------- | ----------------------------------------------------------------------------- |
| `url`          | A string that is coppied to the clipboard and/or used by the native share API. Defaults to the current page's URL |
| `copy-button`  | A string that is used for the copy button text. Defaults to "Copy"                                |
| `share-text`   | A string that is use as the message by the native web share API. Defaults to the current page title               |
| `share-button` | A string that is used for the share button text. Defaults to "Share"                              |
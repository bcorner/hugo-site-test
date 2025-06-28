# Custom Partials

This directory contains custom partials that override the default partials provided by the theme.

## footer.html

This file overrides the default `footer.html` partial to add the site's build date and time to the footer.

It first copies the content of the original footer from the `PaperMod` theme, and then adds the following line to display the build date:

```html
<span>
    Site built on: {{ now.Format "2006-01-02 15:04:05" }}
</span>
```

This uses Hugo's built-in `now` function to get the build date, and then formats it to a more readable string.

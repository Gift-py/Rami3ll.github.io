#

The key files/directories to run/build the **Chirpy** theme are as follows:

```shell
.
├── _data
├── _plugins
├── _tabs
├── _config.yml
└──  index.html
```



[
```

## Usage

### Customing Stylesheet

Creare a new file `/assets/css/style.scss` in your Jekyll site.

And then add the following content:

```scss
---
---

@import "{{ site.theme }}";

// add your style below
```

### Changing the Number of Tabs

When adding or deleting files in the `_tabs` folder, you need to complete the section [Customing Stylesheet](#customing-stylesheet) first, and then add a new line before `@import`:

```scss
$tab-count: {{ site.tabs | size | plus: 1 }};
```


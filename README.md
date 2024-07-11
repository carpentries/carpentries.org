## Carpentries project

For now the theme is local so you can simply run:

1.
```
npm install
```
2.
```
hugo serve
```

## Info

Sepc document: https://docs.google.com/document/d/1yzg1Zes458I8wiDBVKq2ltohRkulwqJbGKxcLriCciM/edit

Expected result: https://deploy-preview-52--carpentries-org-preview.netlify.app/#

## Blocks Logic

Blocks templates live in the `layouts/partials/blocks/templates/{layout}.html` directory where `layout` matches the block's `layout` frontmatter key.

### Example Text Block in Markdown
---
title: New Page
blocks:
- layout: text
  title: Hello World!
  copy: >-
    Fusce dapibus, tellus ac cursus **commodo**, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Lorem ipsum dolor sit amet, consectetur [adipiscing](/url) elit.

    Yep!
---

### Example Text Block template file

At `/layouts/partials/blocks/templates/text.html

```
{{/*
  blocks/text

  @context Map (.)
    Page (.Page)
    Map (.block)
      String (.title)
      String (.copy)

*/}}
{{ with .block }}
  <h3>{{ .title }}</h3>
  {{ with .copy }}
    <div>
      {{ $.Page.RenderString }}
    </div>
  {{ end }}
{{ end }}
```
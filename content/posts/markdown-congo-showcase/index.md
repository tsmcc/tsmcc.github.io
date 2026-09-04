---
title: "Markdown & Congo Feature Showcase"
date: 2026-09-02T09:00:00-04:00
draft: false
build:
  render: always
  list: never
description: "A sample post demonstrating Markdown, Hugo, and Congo theme features."
summary: "A practical gallery of Markdown formatting, Hugo content features, and Congo shortcodes."
images: ["feature.jpg"]
feature: "feature.jpg"
featureAlt: "A Hugo-inspired magenta hexagon combined with the Markdown M and downward arrow symbol"
showTableOfContents: true
showAuthor: true
showReadingTime: true
showWordCount: true
showTaxonomies: false
---

{{< lead >}}
This sample post is a practical tour of Markdown, Hugo, and the Congo theme. It combines placeholder text with formatting examples that can be copied into future posts.
{{< /lead >}}

{{< alert >}}
**Sample content:** This article is intentionally feature-rich. Individual posts only need the elements that serve their subject.
{{< /alert >}}

Status: {{< badge >}}Published with Hugo{{< /badge >}}

## Paragraphs and inline formatting

Lorem ipsum dolor sit amet, consectetur adipiscing elit. **Bold text** draws attention, *italic text* adds emphasis, and ***bold italic text*** does both. Congo also styles ~~strikethrough text~~, `inline code`, and [ordinary links](https://gohugo.io/).

Escaped characters remain literal: \*asterisks\*, \_underscores\_, and \# hash marks. Two trailing spaces create a hard line break.  
This sentence begins on the next line without starting a new paragraph.

You can add useful inline HTML when Markdown alone is not enough: <abbr title="Graphics Interchange Format">GIF</abbr>, H<sub>2</sub>O, x<sup>2</sup>, <mark>highlighted text</mark>, and <kbd>Ctrl</kbd>+<kbd>S</kbd>.

---

## Heading levels

Page titles provide the first-level heading, so article sections normally begin at level two.

### Level-three heading

#### Level-four heading

##### Level-five heading

###### Level-six heading

## Blockquotes and citations

> Lorem ipsum dolor sit amet, consectetur adipiscing elit.
>
> > A nested quotation can provide additional context.
>
> Markdown such as **bold text** and `code` works inside a quote.

> “Simplicity is the soul of efficiency.”  
> — <cite>Austin Freeman</cite>[^quote]

[^quote]: Included as a demonstration of a footnote and citation, not as a claim about the quote's provenance.

## Lists

### Unordered and nested

- Engineering
  - Mechanical systems
  - Electrical systems
  - Control systems
- Technology
  - Linux
  - Networking
  - Local AI

### Ordered

1. Write the content.
2. Preview it with Hugo.
3. Commit the source.
4. Let GitHub Pages deploy it.

### Task list

- [x] Create a Hugo site
- [x] Configure the Congo theme
- [x] Add a custom domain
- [ ] Replace this sample with the next great post

### Definition list

Hugo
: A static site generator that turns content and templates into a deployable website.

Congo
: A responsive Hugo theme with built-in components for rich technical and personal sites.

Markdown
: A lightweight syntax for structured text.

## Tables

| Feature | Syntax | Typical use |
| :--- | :---: | ---: |
| Bold | `**text**` | Emphasis |
| Link | `[label](URL)` | Navigation |
| Code | `` `command` `` | Technical terms |
| Task | `- [x] item` | Checklists |

Markdown works inside cells too: **bold**, *italic*, and `code`.

## Code

Inline commands such as `hugo server` sit naturally within a paragraph.

```toml
baseURL = "https://example.com/"
theme = "congo"
enableRobotsTXT = true
```

The next block uses Hugo syntax highlighting, line numbers, and highlighted lines:

```go {linenos=table,hl_lines=[4,7]}
package main

import "fmt"

func main() {
    message := "Hello from Hugo"
    fmt.Println(message)
}
```

Indented text can also form a code block:

    hugo --gc --minify
    git status --short

## Links and internal references

This is an ordinary link to the [Hugo documentation](https://gohugo.io/documentation/), while this Hugo reference points to the site's [About page]({{< ref "/about" >}}).

{{< button href="/about/" target="_self" >}}
Visit the About page
{{< /button >}}

## Images and figures

Standard Markdown image syntax is supported:

![The tsmccallum.com profile image](/android-chrome-512x512.png "A site image rendered through Markdown")

Congo's figure shortcode adds optimized presentation and a caption:

{{< figure
  src="/android-chrome-512x512.png"
  alt="Profile image used on tsmccallum.com"
  caption="A Congo figure using a root-relative static site image."
>}}

## Congo components

### Alerts

{{< alert "circle-info" >}}
Alerts accept **Markdown**, links, and a configurable Congo icon.
{{< /alert >}}

### Badges and icons

{{< badge >}}Hugo{{< /badge >}}
{{< badge >}}Congo{{< /badge >}}
{{< badge >}}Markdown{{< /badge >}}

Inline icons scale with surrounding text: {{< icon "github" >}} GitHub, {{< icon "mastodon" >}} Mastodon, and {{< icon "email" >}} email.

### Mermaid diagram

{{< mermaid >}}
flowchart LR
  A[Write Markdown] --> B[Build with Hugo]
  B --> C[Deploy with GitHub Actions]
  C --> D[Serve with GitHub Pages]
{{< /mermaid >}}

### Chart

{{< chart >}}
type: 'bar',
data: {
  labels: ['Markdown', 'Hugo', 'Congo', 'GitHub Pages'],
  datasets: [{
    label: 'Sample feature count',
    data: [10, 7, 8, 4],
    backgroundColor: ['#6b7280', '#ec4899', '#8b5cf6', '#3b82f6']
  }]
},
options: {
  plugins: { legend: { display: false } },
  scales: { y: { beginAtZero: true } }
}
{{< /chart >}}

### Mathematical notation

{{< katex >}}

Inline mathematics: \(E = mc^2\)

Block mathematics:

$$
\int_0^1 x^2\,dx = \frac{1}{3}
$$

## Collapsible content and raw HTML

<details>
  <summary>Open this disclosure widget</summary>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante venenatis dapibus posuere velit aliquet.</p>
</details>

## Closing sample

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

The horizontal rule below marks the end of the showcase.

---

*End of sample post.*

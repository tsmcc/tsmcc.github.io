---
title: "{{ replace .File.ContentBaseName "-" " " | title }}"
date: {{ .Date }}
draft: true

# Write these for readers and link previews. Keep the description concise;
# use the summary for article listings when it should differ.
description: ""
summary: ""

tags: []
categories: []

# For a page bundle, place the image beside index.md and uncomment both lines.
# A post without an image will use the site's default portrait for link previews.
# images: ["feature.jpg"]
# feature: "feature.jpg"

showAuthor: true
showReadingTime: true
showTableOfContents: true
showTaxonomies: true
showWordCount: true
---

{{ printf "{{< lead >}}" }}
Write a short opening that tells readers what this article is about and why it matters.
{{ printf "{{< /lead >}}" }}

<!--
Before publishing:
- Replace every prompt in this file.
- Confirm the title, description, summary, tags, and category.
- Add descriptive alt text to every image.
- Check links and preview the page on mobile and desktop.
- Set draft to false only when the post is ready.
-->

## Main idea

Introduce the central point, problem, or question.

## Details

Develop the idea with useful context, examples, evidence, or images.

## Takeaway

Close with the key lesson, recommendation, or next step.

# Sam's website
To edit a file on GitHub, open it, click the pencil icon, make your change, then click **Commit changes**.

| To change | Edit |
| --- | --- |
| About tab | `index.md` |
| Research tab intro | `research.md` |
| Working papers | `_data/papers.yml` |
| Name, email, tabs | `_config.yml` |

**Add a PDF:** click **Add file > Upload files** on the main repo page. Then put the file name after `cv_pdf:` in `_config.yml` (for your CV) or after `pdf:` in `_data/papers.yml` (for a paper).

**Add a tab:** create a page such as `talks.md` with this at the top, then add it under `nav:` in `_config.yml`.

```
---
title: Talks
permalink: /talks/
---
```

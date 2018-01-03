---
title: "Adding a meetup to this site"
date: 2018-01-03T11:58:44+01:00
---

If you know of a meetup you want to add this gopher.community, follow these
steps:

## 1. Create a new page

Each meetup has its own Markdown file stored under
`content/meetup/<country-code>/<meetup-name>.md`.

This file should look like this:

```markdown
---
title: Name of the Meetup
city: City name
country: country code
date: 2018-01-03T11:58:44+01:00
website: https://website.com
---
```

## 2. Add a country entry

Check the `data/countries.yaml` file to see if there is already an entry for
the country the meetup is located in:

```yaml
aut:
    code: aut
    name: Austria
    continent: Europe
```

## 3. Preview

Start the local development server and check the result on
<http://localhost:1313/meetup/>:

```bash
$ hugo serve
```

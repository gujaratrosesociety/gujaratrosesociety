# Gujarat Rose Society

This is a GitHub Pages website for the Gujarat Rose Society, built with Jekyll.

## About

This repository hosts the official website for the Gujarat Rose Society, deployed using GitHub Pages with Jekyll and the Cayman theme. The site is fully bilingual, supporting both Gujarati (ગુજરાતી) and English.

## Viewing the Website

The website is accessible at: https://gujaratrosesociety.github.io/gujaratrosesociety/

## Multilingual Structure

### Supported Languages

- **Gujarati (ગુજરાતી)** - Default language (`gu`)
- **English** - Secondary language (`en`)

### Configuration

The site's language settings are defined in `_config.yml`:

```yaml
default_lang: gu
languages: ["gu", "en"]
```

### File Structure

```
gujaratrosesociety/
├── _posts/                      # Blog posts directory
│   ├── YYYY-MM-DD-post-slug.md           # Gujarati post (no suffix or -gu)
│   └── YYYY-MM-DD-post-slug-en.md        # English post (-en suffix)
├── index.md                     # Gujarati homepage
├── en/
│   └── index.md                 # English homepage
└── _config.yml                  # Site configuration
```

### Blog Post Naming Convention

Blog posts follow Jekyll's standard naming format with language suffixes:

**Format:** `YYYY-MM-DD-post-slug-[LANGUAGE].md`

**Examples:**
- `2026-01-07-understanding-ion-balance-for-roses.md` (Gujarati - no suffix)
- `2026-01-07-understanding-ion-balance-for-roses-en.md` (English - `-en` suffix)

**Language Suffixes:**
- No suffix or `-gu` = Gujarati version
- `-en` = English version

### Post Frontmatter Structure

Every blog post must include YAML frontmatter with these fields:

```yaml
---
layout: post
title: "Post Title in Respective Language"
date: YYYY-MM-DD
categories: space-separated categories
lang: en or gu
---
```

**Example - Gujarati Post:**
```yaml
---
layout: post
title: "ગુલાબ માટે આયન બેલેન્સ સમજવું"
date: 2026-01-07
categories: પોષણ ખાતરો pH આયન-બેલેન્સ
lang: gu
---
```

**Example - English Post:**
```yaml
---
layout: post
title: "Understanding Ion Balance for Roses"
date: 2026-01-07
categories: nutrition fertilizers pH ion-balance
lang: en
---
```

### Language Switcher

The site includes an automatic language switcher in the header that allows users to switch between English and Gujarati while staying on equivalent content.

**How it works:**
- The language switcher matches posts by their slug (removing `-gu` and `-en` suffixes)
- When a user switches languages, they're taken to the same post in the other language
- If no equivalent exists, they're taken to the homepage in that language

**Technical implementation** (`_layouts/default.html`):
```liquid
{% assign current_slug = page.slug | remove: "-gu" | remove: "-en" %}
{% assign alternate_posts = site.posts | where: "lang", alternate_lang %}
{% for alt_post in alternate_posts %}
  {% assign alt_slug = alt_post.slug | remove: "-gu" | remove: "-en" %}
  {% if alt_slug == current_slug %}
    <!-- Link to alternate language post -->
  {% endif %}
{% endfor %}
```

### Adding New Blog Posts

To add a new bilingual blog post:

1. **Create the Gujarati version** in `_posts/`:
   ```
   _posts/YYYY-MM-DD-your-post-slug.md
   ```
   - Include frontmatter with `lang: gu`
   - Write content in Gujarati

2. **Create the English version** in `_posts/`:
   ```
   _posts/YYYY-MM-DD-your-post-slug-en.md
   ```
   - Include frontmatter with `lang: en`
   - Write translated content in English

3. **Ensure matching slugs** (without language suffixes) so the language switcher can pair them

4. **Use the same date and base filename** for both versions

### Homepage Structure

The site has separate homepages for each language:

- **Gujarati Homepage:** `index.md` (root)
  - Filters and displays only posts with `lang: gu`

- **English Homepage:** `en/index.md`
  - Filters and displays only posts with `lang: en`

**Filtering logic:**
```liquid
{% for post in site.posts %}
  {% if post.lang == 'gu' %}
    <!-- Display Gujarati post -->
  {% endif %}
{% endfor %}
```

### Categories

Categories should be provided in the respective language:

- **Gujarati:** પોષણ, માઇક્રોન્યુટ્રિએન્ટ્સ, ખાતરો, pH
- **English:** nutrition, micronutrients, fertilizers, pH

### Best Practices

1. **Always create posts in pairs** - Both languages should have equivalent content
2. **Use consistent slug names** (without language suffixes) to enable language switching
3. **Match publication dates** between language versions
4. **Translate categories** appropriately for each language
5. **Keep frontmatter structure consistent** across both languages
6. **Use proper Unicode** for Gujarati text (UTF-8 encoding)

### Technical Stack

- **Static Site Generator:** Jekyll
- **Theme:** jekyll-theme-cayman
- **Markdown Processor:** kramdown
- **Hosting:** GitHub Pages
- **Languages:** Gujarati (gu) and English (en)


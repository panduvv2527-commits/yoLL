# yoLl --- AI Tools Directory

> **The AI Tools Universe** --- a curated directory for discovering AI
> tools for images, writing, coding, video, audio, research,
> productivity, design, chatbots, agents, marketing, and more.

## What it does

yoLl is a responsive, single-page AI tools directory that lets visitors:

-   🔎 **Search AI tools** by name, description, or category.
-   🗂️ **Filter by category** such as Image, Writing, Coding, Video,
    Audio, Productivity, Research, Design, Chatbots, Marketing, Agents,
    HR, Legal, E-commerce, Data, Translation, and Innovation.
-   💰 **Filter by pricing model** --- Free, Freemium, Paid, or Open
    Source.
-   🔗 **Visit each tool** directly through its external website link.
-   🌓 **Switch between dark and light themes**, with the selected theme
    saved in the browser.
-   📱 **Use the directory on mobile, tablet, and desktop** with
    responsive layouts.
-   ✨ **Browse animated tool cards** with reveal effects and desktop
    hover/3D interactions.
-   ♿ **Respect reduced-motion preferences** for users who prefer less
    animation.
-   🧹 **Handle empty search/filter results** with a reset option.
-   ✅ **Validate tool data** before displaying it and remove duplicate
    tool names.
-   ⚡ **Run entirely as a static webpage** with the tool catalog
    embedded in the HTML.

## Categories

The current catalog contains these categories:

Agents, Audio, Chatbots, Coding, Data, Design, E-commerce, HR, Image,
Innovation, Legal, Marketing, Productivity, Research, Translation,
Video, Writing

## Pricing labels

Each tool is classified using one of these labels:

-   **Free** --- available without a paid plan in the directory's
    classification.
-   **Freemium** --- a free tier is listed, with paid features/plans
    possible.
-   **Paid** --- listed as a paid tool.
-   **Open** --- listed as an open-source/open tool.

> Pricing and availability can change over time. The labels in this
> repository reflect the catalog data currently stored in `index.html`.

## Tech stack

This project is intentionally lightweight:

-   **HTML5** --- page structure and embedded tool data
-   **CSS3** --- responsive layout, themes, animations, cards,
    gradients, and accessibility states
-   **Vanilla JavaScript** --- search, filtering, rendering, theme
    switching, data validation, and interactions
-   **JSON** --- AI tool catalog embedded directly in `index.html`
-   **Google Fonts** --- Inter and Space Grotesk

No frontend framework or build system is required.

## Project structure

``` text
.
└── index.html
```

The tool catalog is stored as JSON inside `index.html`, using fields for
the tool name, description, category, pricing label, URL, and icon.

## Run locally

Because this is a static webpage, you can open `index.html` directly in
a browser.

For a local development server, for example:

``` bash
python -m http.server 8000
```

Then open:

``` text
http://localhost:8000
```

## Adding an AI tool

Add a new object to the `toolsData` JSON array in `index.html`:

``` json
{
  "n": "Tool Name",
  "d": "Short description of what the tool does.",
  "c": "Category",
  "p": "freemium",
  "u": "https://example.com",
  "i": "🤖"
}
```

Supported pricing values are:

``` text
free
freemium
paid
open
```

The built-in validation checks that required fields are present, the
pricing value is supported, and the URL uses HTTP or HTTPS.

## Current features

  Feature                        Status
  ------------------------------ --------
  AI tool directory              ✅
  Search                         ✅
  Category filters               ✅
  Pricing filters                ✅
  Dark/light theme               ✅
  Theme persistence              ✅
  Responsive design              ✅
  External tool links            ✅
  Tool data validation           ✅
  Duplicate-name filtering       ✅
  Loading state                  ✅
  Empty-result state             ✅
  Desktop hover/3D card effect   ✅
  Reduced-motion support         ✅
  Backend required               ❌

## Data

The repository currently includes **176 catalog entries** in
`index.html`, across **17 categories**.

The page describes itself as a curated directory for AI tools covering
images, writing, coding, video, audio and more. The catalog includes
both commercial services and open-source projects.

## Contributing

To contribute:

1.  Fork the repository.
2.  Add or update an AI tool in `index.html`.
3.  Keep descriptions short and factual.
4.  Use the correct category and pricing label.
5.  Make sure the URL is valid and uses HTTPS where available.
6.  Test search and filters in a browser.
7.  Open a pull request.

## License

No license is currently specified in the provided project files. Add a
`LICENSE` file and update this section if you choose a license for the
repository.

## Disclaimer

yoLl is a directory and does not own or operate the third-party AI tools
listed in the catalog. Tool names, descriptions, pricing, availability,
and external links may change. Check each provider's official website
for the latest information.

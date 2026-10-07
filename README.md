# tzachx.github.io

Personal site of Tzach Cohen — gameplay and systems programmer, Tel Aviv.

Live at **[tzachx.github.io](https://tzachx.github.io)**.

Covers current work (Chip Master, a live multiplayer title on Unity WebGL), prior
production C/C++ work, selected personal and jam projects, and a downloadable CV.

## Stack

Static single page. No build step — edit `index.html` and push; GitHub Pages serves `main`.

| Path | Contents |
| --- | --- |
| `index.html` | Entire page: all sections and copy |
| `assets/css/main.css` | Compiled CSS — **edit this**, it is what the page loads |
| `assets/sass/` | SCSS sources, kept for reference; no build step is configured, so they are not compiled on push |
| `assets/js/` | jQuery plus the template's navigation and breakpoint scripts |
| `images/` | Photos, project videos and poster frames |
| `TzachCohenCV.pdf` | CV linked from the Contact section |

## Local preview

```sh
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

## Adding a project

Copy an existing `.project-card` block in `index.html` and replace the video source,
poster, title link, tags and description. Cards without a `<video>` element render
fine — the body simply sits on its own.

## Credits

Built on [Dimension](https://html5up.net/dimension) by HTML5 UP (@ajlkn), used under
the [CCA 3.0 license](https://html5up.net/license). Icons by Font Awesome, fonts by
Google Fonts.

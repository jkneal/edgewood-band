# Edgewood Marching Mustangs

Standalone marketing site for the Edgewood Performing Arts Marching Mustangs —
ISSMA Class C State Champions. Single-page site with three client-side views
(News/Home, Announcements, Forms & itineraries).

Ported from a Claude Design component (`Edgewood Band.dc.html`) to a dependency-free
static site — plain HTML, CSS, and vanilla JS. No build step.

## Structure

```
index.html          All markup, styles, data, and view logic
assets/             Logos (EPA logos). Show/announcement photos load from the
                    Edgewood Squarespace CDN.
render.yaml         Render static-site blueprint
```

## Run locally

Any static file server works. For example:

```bash
python3 -m http.server 8080
# then open http://localhost:8080
```

## Deploy on Render

This repo includes a `render.yaml` Blueprint. On [render.com](https://render.com):

1. **New → Blueprint** and connect this repository, or
2. **New → Static Site**, set **Publish directory** to `.` and leave the build
   command empty.

The site is fully static; no environment variables or build are required.

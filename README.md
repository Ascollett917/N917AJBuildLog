# N917AJBuildLog

Static website for browsing the N917AJ aircraft build log. The home page shows
the latest post from each category; each category links to its own post list in
`category.html`. The site loads entries and categories from `logs/logs.json` and
`logs/categories.json`, and uses the photo paths stored in the log data. The home
page shows the contributors from `logs/contributors.json`, total build hours, and
logged hours for each category. It also links to `documents.html`, which lists
reference PDFs from `logs/documents.json` and links to the separate Van's Plans
page. Van's plan PDFs are listed in `logs/Documents/VansPlans/plans.json` alongside
their files. Posts can also include optional `videos` arrays; video files belong
in `logs/Videos/`.

Open the site from a local web server so the browser can fetch the JSON files.
For example, with Python installed:

```powershell
python -m http.server 8000
```

Then visit <http://localhost:8000>. The repository can also be published as a
static GitHub Pages site from its root.

To add a video to a post, copy an MP4 or WebM file into `logs/Videos/` and add
its path to that post in `logs/logs.json`, for example:

```json
"videos": [
  {
    "filename": "Videos/first-flight.mp4",
    "title": "First flight"
  }
]
```

Click the post title to open its photos and videos. Video playback uses the
browser's built-in controls.


# N917AJBuildLog

Static website for browsing the N917AJ aircraft build log. The page loads entries
and categories from `logs/logs.json` and `logs/categories.json`, and uses the
photo paths stored in the log data. Posts can also include optional `videos`
arrays; video files belong in `logs/Videos/`.

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


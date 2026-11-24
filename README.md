# N917AJBuildLog

Static website for browsing the N917AJ aircraft build log. The page loads entries
and categories from `logs/logs.json` and `logs/categories.json`, and uses the
photo paths stored in the log data.

Open the site from a local web server so the browser can fetch the JSON files.
For example, with Python installed:

```powershell
python -m http.server 8000
```

Then visit <http://localhost:8000>. The repository can also be published as a
static GitHub Pages site from its root.


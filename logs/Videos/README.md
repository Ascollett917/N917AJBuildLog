# Build log videos

Place post video files in this folder, preferably as MP4 (H.264 video with AAC
audio) or WebM. Add each video's path to the post in `../logs.json`:

```json
"videos": [
  {
    "filename": "Videos/first-flight.mp4",
    "title": "First flight"
  }
]
```

The `videos` property is optional. Each video object may include a `title`,
`description`, and optional poster-image path relative to the `logs` folder.
Click the post title on the website to expand its media.

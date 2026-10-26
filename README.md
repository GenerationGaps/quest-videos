# Quest videos

The live list of YouTube videos used in the NGSS quests. Quests read `videos.json` every time they open, so editing a link here changes it for students without re-uploading anything to Canva.

## Changing a video

1. Open `videos.json` and click the pencil icon.
2. Paste the new YouTube link into that video's `"link"`. A full link or just the 11-character ID both work.
3. Click **Commit changes**. Students see the new video within about 5 minutes.

Other fields:
- `start` / `end`: seconds to start and stop at. Use `0` and `null` to play the whole video.
- `mode`: `"required"` locks the next checkpoint until the student starts the video (or opens it on YouTube); `"optional"` lets them skip it.

Keep the quotes and commas exactly as they are. If the file ever breaks, quests fall back to their built-in copy, so students are never stuck.

`video-embed-test.html` is the test page for checking that videos play inside Canva and past Restricted Mode.

---
name: youtube-transcript-local
description: Extract YouTube transcripts (captions first, fallback options) and save clean text files with versioned output in workspace folders. Use whenever user asks for transcript, subtitles, caption extraction, or YouTube-to-text.
---

# YouTube Transcript Local Skill

Use this skill when the user asks to transcribe a YouTube video, extract captions, or save transcript text.

## Workflow

1. Try MCP YouTube transcription tools first:
- list caption languages
- extract transcript in requested language

2. If MCP extraction fails, use CLI fallback with yt-dlp:
- list subtitles with `yt-dlp --list-subs`
- download auto-captions with android client and `srv1`
- clean caption XML to plain text

3. Save outputs in a workspace folder (default: `LinkedInPage/transcripts/`) with versioned filenames:
- `<video_id>.transcript.v1.txt`
- `<video_id>.transcript.v2.txt`

## Local reusable script

A centralized script is available at:
`C:\Users\USER\OneDrive\VSCODESkills\tools\youtube-transcript\extract_youtube_transcript.ps1`

Example usage from any workspace:

```powershell
powershell -ExecutionPolicy Bypass -File "C:\Users\USER\OneDrive\VSCODESkills\tools\youtube-transcript\extract_youtube_transcript.ps1" \
  -Url "https://www.youtube.com/watch?v=0AkQeyG4QmQ" \
  -OutputDir ".\\LinkedInPage\\transcripts" \
  -Language "en"
```

## Output quality notes

- Auto-captions can contain errors.
- If no captions exist, switch to ASR transcription path.
- Preserve raw caption files when troubleshooting.

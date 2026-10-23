# Zendegi pas az zendegi (Life After Life): raw YouTube Persian captions

Raw, unmodified auto-generated Persian captions (WebVTT), plus a plain-text version of each, for 189 episodes of the Iranian TV programme *Zendegi pas az zendegi* (زندگی پس از زندگی, IRIB Channel 4, host Abbas Mowzoon), as published on the YouTube channel "Life After Life | زندگی پس از زندگی".

## Contents
- `transcripts/season_1` ... `season_6`, `season_unassigned`: one `.vtt` file per video, named `<YouTube video id>.fa-orig.vtt`. Season folders follow the channel's season playlists. One video is not in any season playlist and sits in `season_unassigned`.
- `transcripts_txt/season_*`: the same captions as plain text, one `<video id>.txt` per video, same season folders. These are a mechanical conversion of the `.vtt` files: timing tags removed and the rolling-caption repeats collapsed into a single running line of text. Words, punctuation and non-speech tags such as `[موسیقی]` are untouched. Each file was checked against an independent re-extraction from its `.vtt` (189 of 189 identical). The `.vtt` files remain the primary source.
- `metadata.csv`: video id, season, title, duration (seconds), upload date, URL and file paths (`file` = vtt, `txt_file` = txt) for every video (UTF-8 with BOM, opens correctly in Excel).
- `SHA256SUMS.txt`: checksum of every `.vtt` and `.txt` file, to verify the files are unchanged (`sha256sum -c SHA256SUMS.txt`).

## Provenance
- Source: the YouTube auto-generated caption track `fa-orig` (original-language Persian speech recognition), downloaded with yt-dlp in October 2026. All 189 videos had this track.
- The `.vtt` files are exactly as downloaded: no cleaning, no editing, no speaker labels, no coding. The `.txt` files add nothing beyond the conversion described above.
- `upload_date` is the date shown by YouTube. Several 2024 episodes were re-uploaded in 2025-2026, so upload date is not the broadcast date.

## Known properties of the raw files
- **Machine transcription.** The text is speech-recognition output with no human correction. Expect mis-hearings, missing or wrong punctuation, and errors in names, numbers and religious or Arabic terms.
- **No speakers.** Host, guest, narrator and archival clips are not distinguished.
- **WebVTT rolling-caption format.** Each cue repeats the previous line and carries word-level timing tags (`<00:00:17.840><c> ...</c>`), so the same text appears several times. Non-speech tags such as `[موسیقی]` (music) are included.
- **Repeated content.** The programme replays clips and recaps between episodes, and at least three videos are exact re-uploads of other videos in this set (identical title and text). Nothing was removed.

## Rights and licence
The compiler dedicates this compilation to the public domain under [CC0 1.0](LICENSE): the selection and arrangement of the files, `metadata.csv`, `SHA256SUMS.txt`, the plain-text conversion and this README. Anyone may copy, modify and reuse them without asking permission or giving credit.

The dedication covers only the compiler's own rights. The captions are automatic speech-recognition output of IRIB broadcasts published on a YouTube channel, and the compiler cannot waive rights that other parties may hold in the programme itself. The files are shared as publicly available research data.

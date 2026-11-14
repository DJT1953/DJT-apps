# DJT Apps

Free, simple Windows programs. Each one comes as a single **Setup.exe** that brings
everything it needs, so you don't have to install Python or anything else first.

## Download

Go to **[Releases](../../releases)** and download the Setup.exe for the app you want.

| App | What it does |
|---|---|
| Video Player | Plays MP4, MKV, AVI, MOV and most other videos, a whole folder at a time. Full screen, skip 10 s, save a frame as a picture. |
| Video Editor | Cuts and joins videos and sound files, with volume, fades and added music, then saves a new MP4, MP3 and more. |
| Audio Editor | Plays and edits MP3, WAV, FLAC and other sound files on a waveform: cut, copy, paste, change the voice, add effects, record, and save. |
| Photos to Word | Turns photos of printed pages into Word files you can edit. Pick a folder of photos; the text is read and laid out like the page. |
| Combine Word Files | Joins every Word file in a folder into one, in page-number order, each keeping its own look. |
| Document Reformatter | Gives every Word, RTF and text file in a folder one new font, size and spacing, saving copies. **Needs Microsoft Word.** |
| Document Renamer | Renames a folder of files at once: from their first words, old names or your own text, with dates and numbers. Undo puts old names back. |
| Find and Replace | Changes text in many Word, RTF and text files at once: words, formatting, beginnings, endings and sections between two phrases. Shows every change first. **Needs Microsoft Word for Word and RTF files.** |
| Cross Folder Compare | Finds the photos and documents two folders have in common, even renamed, resized or re-saved. Never moves or deletes anything. |
| Duplicate File Finder | Finds exact copies and look-alike photos, videos and documents, and moves the extras to a review folder. Never deletes anything. |
| Clean Up Scans | Straightens, crops and whitens photographed or scanned pages, saving cleaned copies and leaving the originals alone. |
| Proofreader | Fixes spelling, grammar, punctuation and capitals in Word, RTF and text files, saving corrected copies with a report. Its free checker works offline; Word is optional. |
| Song Cleaner | Tidies a folder of MP3s recorded from the radio: better names, copies of the same song removed, talk trimmed from the ends. Nothing is deleted; Undo puts it back. |

More apps are on the way.

## Before you install

- **Windows 10 or 11, 64-bit.** The apps don't run on Mac, Linux or 32-bit Windows.
- **"Windows protected your PC."** The installers aren't code-signed (signing is a paid yearly service), so Windows may show this blue box the first time. Click **More info**, then **Run anyway**.
- **Antivirus warnings.** A few antivirus programs wrongly flag new, unsigned programs. Each download page lists the file's SHA-256 fingerprint, so you can check you have the real file: in PowerShell, type `Get-FileHash` followed by the file's name, and compare.
- **Microsoft Word.** Document Reformatter needs Microsoft Word, which isn't included. Document Renamer needs Word or the free LibreOffice only to name files from the words inside Word and RTF files. Proofreader works without Word on .docx and .txt files; only .doc and .rtf files need it. Find and Replace needs Word for Word and RTF files; .txt files work without it. Their Setup tells you if these aren't found.
- **No administrator password needed.** Apps install to `C:\Users\<you>\DJT_Code\<app name>`.

## Install

1. Double-click the Setup.exe.
2. Windows may show a blue box saying **"Windows protected your PC"** because the app isn't
   from a big company. Click **More info**, then **Run anyway**.
3. Click **Next** a few times. No administrator password is needed.

Apps install to `C:\Users\<your name>\DJT_Code\<app name>`, with a Desktop shortcut and a
Start menu entry.

## Remove

Settings > Apps > Installed apps > pick the app > **Uninstall**.

## Licenses

The apps are free. They are built with free parts such as Python, Qt (PySide6), FFmpeg, Tesseract OCR, OpenCV, LanguageTool, Java (Eclipse Temurin), mutagen and Chromaprint. Their licenses,
and where to get their source code, are in the `licenses` folder inside each installed app.

Song Cleaner is free software under the GNU GPL (version 3 or later). Its source code comes with it, in the `source` folder of the installed app, and as a zip on its release page.

## For download sites

Each app has a PAD file (Portable Application Description 4.0) in the [`pad`](pad) folder,
with screenshots and icons in [`images`](images). Download sites may list the apps and
offer the unchanged Setup.exe files.

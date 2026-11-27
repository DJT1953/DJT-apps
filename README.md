# DJT Apps

Free, simple Windows programs. Each one comes as a single **Setup.exe** that brings
everything it needs, so you don't have to install Python or anything else first.

## Download

Go to **[Releases](../../releases)** and download the Setup.exe for the app you want.

Each app has a **Check for updates** button that opens [the page with the newest version of every app](https://djt1953.github.io/office-tools-and-learning-games/).

| App | What it does |
|---|---|
| Video Player | Plays MP4, MKV, AVI, MOV and most other videos, a whole folder at a time. Full screen, skip 10 s, save a frame as a picture. |
| Music Player | Plays the music on your PC, about 50,000 internet radio stations, and Spotify, with big buttons and big words. Sleep timer included. |
| Book Reader | Reads EPUB, Kindle (MOBI, AZW, AZW3), PDF and text books, with a library of covers, bookmarks, notes, search and reading aloud. |
| Screen Recorder | Films your whole screen with the computer's sound and your voice into one MP4. Ctrl+Alt+R starts it from any program; Esc stops and saves. |
| Video Editor | Cuts and joins videos and sound files, with volume, fades and added music, then saves a new MP4, MP3 and more. |
| Audio Editor | Plays and edits MP3, WAV, FLAC and other sound files on a waveform: cut, copy, paste, change the voice, add effects, record, and save. |
| Photos to Word | Turns photos of printed or handwritten pages into Word files you can edit. Pick a folder of photos; the text is read and laid out like the page. |
| Combine Document Files | Joins Word and RTF files into one, in the order you choose, each keeping its own look. Tick the files to join; save as .docx, .doc, .rtf or PDF. (Called Combine Word Files up to 1.0.1.) |
| Document Reformatter | Gives every Word, RTF and text file in a folder one new font, size and spacing. Joins lines broken at every line end and splits giant run-together paragraphs. The originals are kept, unchanged, in an Originals folder. **Needs Microsoft Word.** |
| Document Renamer | Renames a folder of files at once, or just the ones you pick: from their first words, old names or your own text, with dates and numbers. Tick boxes leave any file out; Undo puts old names back. |
| Find and Replace | Changes text in many Word, RTF and text files at once: words, formatting, beginnings, endings and sections between two phrases. Shows every change first. **Needs Microsoft Word for Word and RTF files.** |
| Cross Folder Compare | Finds the photos and documents two folders have in common, even renamed, resized or re-saved. Can move the extra copies into a REMOVED BY DUPLICATE SCAN folder by one rule (keep the newer, older, bigger, smaller or sharper copy), with Undo. Never deletes anything. |
| Duplicate File Finder | Finds exact copies and look-alike photos, videos and documents, and moves the extras to a review folder. Never deletes anything. |
| Clean Up Scans | Straightens, crops and whitens photographed or scanned pages, saving cleaned copies and leaving the originals alone. |
| Proofreader | Fixes spelling, grammar, punctuation and capitals in Word, RTF and text files, saving corrected copies with a report. Its free checker works offline; Word is optional. |
| Song Cleaner | Tidies a folder of MP3s recorded from the radio: better names, copies of the same song removed, talk trimmed from the ends. Nothing is deleted; Undo puts it back. |
| Photo Stitcher | Joins overlapping photos into one big panorama, in any order: side by side, top to bottom, or in rows and columns. Trims the ragged edges; an Adjust window turns, squares up, crops and resizes it. Opens iPhone HEIC photos. Your photos are never changed. |
| Dating Photographs | Reads the dates written on old photos (front, border or back, even in handwriting) and renames each one, or a copy of it, by its date, like 1998-10-01.jpg. You check every date first; it can also set Date taken and print the date in orange like a film camera. Undo puts everything back. |


## Before you install

- **Windows 10 or 11, 64-bit.** The apps don't run on Mac, Linux or 32-bit Windows.
- **"Windows protected your PC."** The installers aren't code-signed (signing is a paid yearly service), so Windows may show this blue box the first time. Click **More info**, then **Run anyway**.
- **Antivirus warnings.** A few antivirus programs wrongly flag new, unsigned programs. Each download page lists the file's SHA-256 fingerprint, so you can check you have the real file: in PowerShell, type `Get-FileHash` followed by the file's name, and compare.
- **Microsoft Word.** Document Reformatter needs Microsoft Word, which isn't included. Document Renamer needs Word or the free LibreOffice only to name files from the words inside Word and RTF files. Proofreader works without Word on .docx and .txt files; only .doc and .rtf files need it. Find and Replace needs Word for Word and RTF files; .txt files work without it. Book Reader uses Word only to save a copy of a book as Word. Their Setup tells you if these aren't found. Combine Document Files needs Word only to read .doc and .rtf files and to save as .doc, .rtf or PDF; .docx files work without it.
- **No administrator password needed.** Apps install to `C:\Users\<you>\DJT_Code\<app name>`.

## Install

1. Double-click the Setup.exe.
2. Windows may show a blue box saying **"Windows protected your PC"** because the app isn't
   from a big company. Click **More info**, then **Run anyway**.
3. Click **Next** a few times. No administrator password is needed.

Apps install to `C:\Users\<your name>\DJT_Code\<app name>`, with a Desktop shortcut and a
Start menu entry.

## Update

Download the new version's Setup.exe and double-click it. There is no need to uninstall the
old version first: Setup replaces it in the same folder and keeps your settings.

## Remove

Settings > Apps > Installed apps > pick the app > **Uninstall**.

## Licenses

The apps are free. They are built with free parts such as Python, Qt (PySide6), FFmpeg, RapidOCR (ONNX Runtime), OpenCV, pillow-heif (libheif, x265), LanguageTool, Java (Eclipse Temurin), mutagen, Chromaprint and soundcard. Their licenses,
and where to get their source code, are in the `licenses` folder inside each installed app.
Document Reformatter, Document Renamer and Find and Replace use only parts that come with Windows,
so they have no `licenses` folder.

Song Cleaner, Music Player and Photo Stitcher are free software under the GNU GPL (version 3 or later). Their source code is a zip on each of their release pages; Song Cleaner and Music Player also install it in their `source` folder.

## For download sites

Each app has a PAD file (Portable Application Description 4.0) in the [`pad`](pad) folder,
with screenshots and icons in [`images`](images). Download sites may list the apps and
offer the unchanged Setup.exe files.

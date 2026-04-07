# Spotify Data Viewer

A simple, modern, single-page HTML viewer for your Spotify data export. Runs entirely in your browser — no data is uploaded anywhere.

## License & Commercial Use

This project is dual-licensed.

- **Open Source:** Free to use under the GNU AGPLv3 for open-source and hobbyist projects.
- **Commercial:** If you wish to use this code in a proprietary (closed-source) product or simply want to support the development, you must purchase a Commercial License. Reach out via [GitHub](https://github.com/joetomkinson) or [LinkedIn](https://www.linkedin.com/in/joetomkinson/).

All contributions are subject to the repository CLA. By contributing, you agree that the maintainer may relicense your contribution under commercial terms as described in [CONTRIBUTING.md](CONTRIBUTING.md) and [CLA.md](CLA.md).

## Live Demo

👉 **[Try it here](https://joetomkinson.github.io/spotify-data-viewer/)** — click "Try with Demo Data" to explore with sample data.

### Screenshots

<img width="1080" alt="image" src="https://github.com/user-attachments/assets/5bf0db72-f8a5-41d2-b97e-e2c68ff1fee5" />
<img width="1080" alt="image" src="https://github.com/user-attachments/assets/1394d16d-ed64-4e06-a79f-656e5274357b" />
<img width="1080" alt="image" src="https://github.com/user-attachments/assets/5d73320d-29cb-44d7-842f-ca08d82e6343" />
<img width="2206" height="1246" alt="image" src="https://github.com/user-attachments/assets/118a5fc4-cc82-4cb9-aaf6-c2df66516501" />

## Features

- **Drag & drop** your Spotify export folder or select individual JSON files
- **Streaming History** — sortable, searchable, paginated (handles thousands of streams)
- **Your Library** — browse saved tracks, artists, and albums with tab switching
- **Playlists** — click any playlist to browse its tracks
- **Wrapped** — supports multiple years (Wrapped2024, Wrapped2025, etc.) with year switcher
- **Podcasts, Search History, Sound Capsule** — all browsable
- **Follows** — see who you follow and who follows you
- **Inferences** — view the advertising audience segments Spotify assigned to you
- **Data Sources** — overview of all loaded files with record counts and date ranges
- **100% client-side** — everything runs in your browser, nothing leaves your machine
- **Single HTML file** — no build tools, no dependencies, no server needed

## How to Get Your Spotify Data

1. Go to [Spotify Privacy Settings](https://www.spotify.com/account/privacy/)
2. Scroll down to **"Download your data"**
3. Request your data (Spotify will email you when it's ready)
4. Download and unzip — you'll find a folder called **Spotify Account Data** containing JSON files

## Usage

### Option 1: Use the hosted version

Visit the live demo link above and drop your files onto the page.

### Option 2: Run locally

1. Download `index.html`
2. Open it in any modern browser
3. Drop your Spotify JSON files onto the page, or click "Select Folder"

## File Support

The viewer recognises these Spotify export files:

| File                              | Content                       |
| --------------------------------- | ----------------------------- |
| `StreamingHistory_music_*.json`   | Music listening history       |
| `StreamingHistory_podcast_*.json` | Podcast listening history     |
| `Playlist*.json`                  | Your playlists and tracks     |
| `YourLibrary.json`                | Saved tracks, artists, albums |
| `Wrapped*.json`                   | Wrapped data (any year)       |
| `SearchQueries.json`              | Search history                |
| `Follow.json`                     | Following / followers         |
| `Userdata.json`                   | Account info                  |
| `Identity.json`                   | Display name and profile      |
| `Inferences.json`                 | Ad-targeting segments         |
| `Marquee.json`                    | Artist recommendations        |
| `YourSoundCapsule.json`           | Weekly listening snapshots    |

## Privacy

This tool processes everything locally in your browser using the [File API](https://developer.mozilla.org/en-US/docs/Web/API/File_API). No data is sent to any server. The demo data in `demo-data/` is fully anonymised.

## License

GNU AGPLv3 for open-source use, with commercial licensing available separately. See [LICENSE](LICENSE), [CONTRIBUTING.md](CONTRIBUTING.md), and [CLA.md](CLA.md).

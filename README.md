# PosterPlayer

PosterPlayer is a Windows desktop application for managing and displaying movie and television poster artwork on a dedicated display.

## Current Release

PosterPlayer 1.2.0 is the current stable release. It is a self-contained 64-bit Windows desktop application built with C#, .NET 10, and WPF.

The application is currently unsigned by design.

## Current Features

- Curated local movie and television poster libraries
- Multiple posters per title, Preferred Posters, and metadata editing
- Manual and rule-based Smart Playlists
- Local folder and playlist playback
- Resizable Preview and dedicated-display playback
- Configurable poster duration, transitions, and transition randomization
- Online poster discovery using TMDB and Fanart.tv
- Manual and online poster importing
- Automatic managed poster filename organization
- Local backup and restore
- Optional launch at Windows sign-in

## What's New in 1.2.0

PosterPlayer 1.2.0 introduces a unified **Media Integrations** area for Kodi, Jellyfin, Emby, and Plex.

- Read-only provider Library Browsers for Movies and parent Television Series
- Movie and Television Series matching with PosterPlayer titles
- Provider poster and genre import/update workflows
- Optional Now Playing poster overrides with temporary provider artwork fallback
- Independent integration and Now Playing settings for each provider
- Stable handling of multiple providers and playback sessions
- Provider-library search and filtering by match status, year, decade, and genre
- Clearer Showing, Matched, and Not matched counts and improved follow-up workflows
- Centralized **Tools > Backup & Restore** and **Tools > Diagnostics & About**
- Expanded Help and provider troubleshooting
- Improved Light and Dark theme consistency, including themed Cut, Copy, and Paste menus

When a Now Playing override is enabled, PosterPlayer can temporarily replace its normal rotating poster with artwork corresponding to media playing through a configured integration. Normal poster rotation resumes when playback ends.

## Media Integrations

- **Kodi** integrates through Kodi's JSON-RPC interface.
- **Jellyfin** uses the configured server, API credential, and monitored user for supported library browsing and playback-status monitoring.
- **Emby** uses the configured server, API credential, and monitored user for supported library browsing and playback-status monitoring.
- **Plex** uses the configured Plex server, token, and account for supported library browsing and playback-status monitoring.

All provider libraries are read-only from PosterPlayer's perspective. PosterPlayer observes playback status for poster-display behavior; it does not start, stop, pause, resume, or otherwise control provider playback.

## Application Navigation

PosterPlayer's main areas are:

1. Player
2. Library
3. Artwork Sources
4. Media Integrations
5. Playlists
6. Transitions
7. Tools
8. Help

## Project Status

PosterPlayer 1.2.0 is a final, stable release. The source code and continued development are maintained privately.

This public repository provides product information only. It does not contain PosterPlayer source code or release binaries.

## Local Data and Privacy

PosterPlayer stores its library, settings, and managed posters locally. Credential values are stored separately using Windows Credential Manager and are not included in PosterPlayer backups.

**Tools > Backup & Restore** provides normal backup and restore operations. **Tools > Diagnostics & About** provides application and version information, sanitized diagnostics, credits, and notices. Copied diagnostics omit secret credential values and authorization data.

## Artwork and Metadata

PosterPlayer can use external artwork services to locate movie and television poster artwork.

This product uses the TMDB API but is not endorsed or certified by TMDB.

Fanart.tv is also supported as an optional artwork provider.

PosterPlayer does not redistribute artwork as part of the application.

Kodi, Jellyfin, Emby, and Plex are separate projects, products, or services. PosterPlayer is not affiliated with or endorsed by those providers.

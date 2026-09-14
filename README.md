# HTOpt-Opponent-Analyzer
Local Windows CHPP desktop app for reviewing the recent formation history of your next two Hattrick opponents.
**HTOpt Opponent Analyzer** is a lightweight, read-only Windows desktop application for Hattrick managers.

It connects to Hattrick through CHPP OAuth, shows all senior teams owned by the authorized manager, displays the next two scheduled opponents for the selected team, and lets the manager review the recent formation history of one selected opponent at a time.

> **CHPP status:** This project is currently being prepared for Hattrick CHPP product/function approval. It does not claim final CHPP approval yet and does not display the official CHPP logo.

## Features

- **All owned senior teams**  
  After authorization, the application lists all senior teams linked to the manager. The user explicitly chooses which team to inspect.

- **Next two opponents**  
  Shows the selected team's next two scheduled matches, including:
  - opponent
  - match date
  - home/away status
  - competition type

- **On-demand opponent formation history**  
  The user can manually analyze either of the next two opponents. Only one opponent's statistics are displayed at a time.

- **Recent match history only**  
  Formation history is limited to:
  - the previous **16 weeks**
  - a maximum of **32 matches**

- **Useful filters**  
  Formation history can be filtered locally by:
  - All / Home / Away
  - All / League / Cup / Friendly

- **52 interface languages**  
  The application includes language options for:
  Albanian, Arabic, Basque, Belarusian, Bosnian, Brazilian Portuguese, Bulgarian, Catalan, Chinese, Croatian, Czech, Danish, Dutch, English, Estonian, Finnish, Flemish, French, Frisian, Friulano, Galician, Georgian, German, Greek, Hebrew, Hungarian, Icelandic, Italian, Japanese, Korean, Latvian, Lithuanian, Luxembourgish, Macedonian, Maltese, Norwegian, Norwegian Nynorsk, Persian, Polish, Portuguese, Romanian, Russian, Serbian, Slovak, Slovenian, Spanish, Spanish Central American, Spanish South American, Swedish, Turkish, Ukrainian and Vietnamese.

## Download

Open the **Releases** section of this repository and download the latest Windows release.

For v1.0.0, the recommended package is:

`HTOpt-Opponent-Analyzer-v1.0.0-Windows.zip`

The standalone executable is also provided:

`HTOpt Opponent Analyzer v1.0.0.exe`

## Requirements

- Windows 10 or Windows 11
- Internet connection when communicating with Hattrick CHPP
- A modern web browser

No Python installation and no external server are required.

## How to use

1. Download and extract the Windows release.
2. Run `HTOpt Opponent Analyzer v1.0.0.exe`.
3. Your default browser opens a local address such as `http://127.0.0.1:8765`.
4. Select **Connect to Hattrick**.
5. Authorize the application using Hattrick's official CHPP OAuth page.
6. Copy the verifier code from Hattrick back into the local application.
7. Select one of your senior teams.
8. Choose one of the next two opponents and select **Analyze Opponent**.
9. Filter the formation history by venue and competition if needed.

## Privacy

HTOpt Opponent Analyzer is designed to run locally on the user's computer.

- The browser communicates with the application through `127.0.0.1`.
- Hattrick data is requested directly through CHPP.
- The user's Hattrick password is never requested or stored.
- CHPP authorization data is stored locally on the user's computer.
- No analytics or telemetry service is included.
- Opponent analysis is not uploaded to an HTOpt-hosted server.
- There is no central opponent-history database in this desktop release.

Local application data is normally stored under:

`%LOCALAPPDATA%\HTOpt Opponent Analyzer\`

Using **Logout** removes the locally stored CHPP authorization for the application profile.

The v1.0.0 executable may be unsigned. Windows SmartScreen may therefore display an unknown-publisher warning even when the file was downloaded from the official repository.

## CHPP usage

The application identifies itself to Hattrick as:

`User-Agent: HTOpt Opponent Analyzer/1.0.0`

Downloads of opponent history are initiated explicitly by the user. The application does not perform background polling or automatic opponent downloads.

## Platform

Current public release:

**Windows — v1.0.0**

## Source code

This repository is used as the public product and release page for HTOpt Opponent Analyzer. The application is distributed as a compiled Windows desktop application. The source code is not published as part of the public v1.0.0 release.

## Disclaimer

HTOpt Opponent Analyzer is an independent third-party application for Hattrick.

Until Hattrick completes the final CHPP approval process, this repository and the application do not claim to be an officially approved CHPP product and do not use the official CHPP logo.

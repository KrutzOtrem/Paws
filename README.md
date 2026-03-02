<!-- ————————— HEADER ————————— -->
<h1 align="center">
  🐈‍⬛ Paws, Productivity and Workflow System
</h1>

<!-- minimal jump-<img src="https://github.com/user-attachments/assets/44abbcda-a786-4b9f-91cb-46cf99003799" height="20">s bar -->
<h3 align="center">
  <a href="#timer-quick-menu">Timer</a>&nbsp;•&nbsp;
  <a href="#protocol-menu">Protocol</a>&nbsp;•&nbsp;
  <a href="#settings-main-menu">Settings</a>&nbsp;•&nbsp;
  <a href="#stillroom-keybind-reference">Keybinds</a>&nbsp;•&nbsp;
  <a href="#credits">Credits</a>
  
</h3>

Paws is a distraction-free focus app for NextUI that pairs Pomodoro sessions, daily schedules, and music integration with a system that turns your focus time into budgeted gaming sessions. It comes with an unimpressed cat. 

## 📱 Screenshots
<p>

<table width="100%" cellspacing="0" cellpadding="4" border="1">
  <tr>
    <td width="33%" align="center">
      <img src="https://github.com/user-attachments/assets/9a378fd8-bad5-49e5-8725-e1cc3c5cb97a" width="100%"><br>
       <sub><em>Main Screen</em></sub>
    </td>
    <td width="33%" align="center">
      <img src="https://github.com/user-attachments/assets/ac11252d-0b35-43d1-8ea6-0ff4ae805a6c" width="100%"><br>
      <sub><em>HUD Hidden</em></sub>
    </td>
    <td width="33%" align="center">
      <img src="https://github.com/user-attachments/assets/9ea71b13-a3ee-48a3-9197-aa11b0e681d1" width="100%"><br>
      <sub><em>Terminal</em></sub>
    </td>
  </tr>
   <tr>
    <td width="33%" align="center">
      <img src="https://github.com/user-attachments/assets/9e5efd98-7a33-42a5-a5c5-8b82496920d21" width="100%"><br>
       <sub><em>Pomodoro</em></sub>
    </td>
    <td width="33%" align="center">
      <img src="https://github.com/user-attachments/assets/be23d399-c2dd-4d8a-9737-613257c6ed1a" width="100%"><br>
      <sub><em>Routines</em></sub>
    </td>
    <td width="33%" align="center">
      <img src="https://github.com/user-attachments/assets/6a0613bd-3b5b-414c-b361-e0fdd8cf15c7" width="100%"><br>
       <sub><em>Purrcade</em></sub>
    </td>
  </tr>
</table>

## 🎯 Objective



At its core, Paws is a simple focus and time-management app for NextUI. I built it because I wanted a place to focus without using my phone as the center of that process. Phones are surely useful, but they are also where distraction lives.

Indeed, for years, I noticed my attention span getting worse. Even without social media, I still had the same pattern of checking my mails, looking up random things, losing contexts, restarting.

I’ve tried what feels like every focus and productivity app in existence. The serious ones, the lo-fi ones, the gamified ones. Simple timers, full-blown narrative games, anything with a Pomodoro timer built in. After years of testing and actually using them, this is probably the only topic where I can confidently call myself an expert.

Many of those apps are clearly made with care, and they absolutely work for most people. Unfortunately, not for me. My mind throws up constant, random thoughts at me; some are real inspirations related to my work, but they're distractions nevertheless. A task that should take one hour turns into two or three because I start researching, checking the time, reading emails, or chasing `a super important topic before I forget`. In practice, this is noise, and frankly, a genius trick by the brain to avoid staying still and focusing.

That is also why I picked this device format: you cannot truly multitask on it, so it is much harder to distract yourself. I also disabled music browsing behavior as much as possible, because my brain turned that into another avoidance pattern by constantly searching for the perfect track instead of focusing.

Paws started as a simple Pomodoro timer, and only as a timer, with no text label attached. Over time, I kept adding what I actually needed during real sessions: better tracking, visuals, music, and a system that actually tricks me, for once, into playing games on Brick. I don’t claim this is better than what already exists. It has plenty of faults, most of them stemming from my own limitations, but it undeniably separates the self from the phone, which, in my opinion, has great value.

That is still the point of this app.

## Main Screen

The Main Screen is the center of Paws: timer state, focus status, music state, backgrounds, and quick access to the app's major flows.

Core purpose:

- Focus sessions with clear start/pause/resume flow
- Background and mood control without leaving the session context
- Music and ambience control without turning the app into a full media browser
- Lightweight HUD plus optional text customizations

What you are seeing here in practice comes from four systems that work together:

- Focus sessions (Pomodoro + custom timer)
- Meditation
- Atmosphere and visual customization
- Music playback

## Timer Quick Menu

### ⏱️ Timer

Custom timer supports countdown or count-up and can be labeled for session tracking. Session history and stats are saved so you can see where your time actually went.

### 🍅 Pomodoro

Pomodoro session setup and loop flow with saved behavior that is designed to be simple and repeatable.

### 🧘 Meditation

Meditation includes three modes:

- Timed meditation with interval bells
- Guided meditation audio
- Guided box-breathing mode with visual pacing

### 📒 Tasks

Tasks are simple checklists with completion tracking. This stays intentionally lightweight.

### 🕑 Routines

Routines provide day and time-of-day planning with phase structure:

- Morning
- Afternoon
- Evening
- Night

And weekly scheduling from Monday to Sunday.

### 📖 Booklets

Booklets are plain text quick-reference files shown inside the app. They read `.txt` files from the `booklets/` folder.

- Although there is no full Markdown support, the following styles are recognized: *italics*, **bold**, # h1, ## h2, ### h3, [main], [accent], and [highlight].


## Protocol Menu

Protocol is optional, but it is also the most distinctive part of Paws because it connects focus tracking to your game library.

### 🐈‍⬛ Terminal

Terminal is the guidance interface, run by a cat who leans on sarcasm a bit too much. His name is Paws, and he is the purroductivity and workmeow system itself, as he calls it.

- Paws is the guidance interface. It continuously logs your focus and meditation sessions, then converts that history into two practical values: recuperation minutes (that you purchase tickets for game sessions with) and progression. You can run this system strictly, keep it looser, or manually add and subtract time depending on how rigid you want the loop to be.

- Guidance manages up to three active quests at a time, excluding narrative questlines. Each quest is a concrete play objective tied to a game, system, or achievement, and this is where recuperation minutes are actually spent. Recommendations are pulled from your ROM library and can be limited by your system whitelist. Quests can be generated automatically or selected manually through Protocol.

- When RetroAchievements data is available, Paws attaches the first locked achievement for the selected game. If that data is unavailable, it falls back to a time-based objective. Abandon behavior is intentionally restricted: a quest can only be abandoned after at least five minutes of play, and only if no achievement has been unlocked.
  - For RetroAchievements-only assignments, I suggest scanning RA-only games under Settings → RetroAchievements. Otherwise, Paws will look for an achievement and fall back to generic quests if none are available. This happens because achievement calls are generated only after a random game is selected, as there’s no feasible way around that. I did implement a partial workaround by blacklisting games that have no RetroAchievements in the database, so when a game is randomly picked, it will naturally favor one with achievements. This is why scanning your ROM directories is helpful, though less necessary if your library mostly consists of popular games that already support achievements.
  - Cross-checking your ROM directory against the RetroAchievements database requires a WebAPI key. These keys are long strings of numbers and letters and aren’t practical to enter using the embedded keyboard. Please open `./states/config.txt` and edit the line containing `ra_api_key=` to add your key manually.
    - Under RetroAchievements settings, navigate to Authentication to find your API key. 

- Paws also hosts built-in and custom narrative guidance, which is predefined narrative content written by me and delivered through this flow. Narrative chains take time to design, write, and test, so updates are planned regularly but not rushed. They are basically one long quest chain (10 stages) centered on RetroAchievements objectives.

- Custom narratives are plain `.txt` files under `terminal/narratives/`, using an INI-style format with a `[meta]` block and staged nodes (`stage.N.*`). Supported task types are `play_game`, `play_console`, and `earn_achievement`, and these can be combined across stages. A typical quest chain is structured as intro, optional user branch, objective, then completion text. I encourage people to write and share narratives, mostly because it is fun to do, but especially now that RetroAchievements support is in place, and community-made quests can be a fun thing. I also built a node-based quest editor so anyone can create these quests, so please check it out [here](https://krutzotrem.github.io/stillroom-editor/) (this is an outdated build, but I will update the version when I find the time). RetroAchievements is my own port, so some edge-case behavior may differ slightly and you many encounter bugs (I hope you don't). Core functionality is the same, so these narrative quests can be completed within Paws, or within NextUI's own MinArch.


### ⌛ Balance

Balance manages recuperation minutes and minute economy behavior.

- Recuperation behavior is adjustable (rate + manual add/subtract)
- You can use Stillroom as a pure focus app, or use guidance only by manually adding time

### 👓 Simulations

Simulations are controlled play sessions inside the same ecosystem.

- Claimed balance minutes can be used for intentional, controlled play windows
- Minute countdown and remaining-time tracking are controlled by my customized MinArch (what Paws calls it, Purrcade)
- To make time tracking work correctly, launch games from Paw's Protocol/quest flow inside the PAK (not directly from NextUI's own)
- It is a simplified fork with Paws-specific modules, including RetroAchievements integration, online manual and game logo support, and a custom overlay system

### 💓 Stress Test

Stress Test is a stricter challenge behavior for users who want harder rules than regular simulation sessions. Normally supports hardcore RetroAchievements, but I disabled it until the implementation is more complete and we get an okay from the developers.

### 📔 Protocols

Protocols are basically the quest board.

### 🧍 Baseline

Baseline keeps records of your focus/meditation sessions.

I must say, if you only want timers, routines, meditation, and stats, you do not have to interact with this system at all.

## Settings Main Menu

### 🧑 Profile

Profile includes user/account-facing settings and service pairing details.

Spotify notes:

1. Create a folder under `music/` and use `album.spotify` with the album URL.
2. In Paws, open `Settings -> Profile -> Spotify`, set your device name (however you want), and use `connect / restart`.
3. Pair from a signed-in phone or computer: start playback there first, open Spotify's device picker, and select your device name.
4. After pairing, Spotify issues tokens for playback control. These are not permanent and may expire or be revoked.
5. You don't need to pair it every time to use it, but I also don't know how long it can be stored for.
6. Paws and your device will be in sync, which means you can continue listening on your mobile/computer, but not vice versa. That would defeat its purpose.
7. Spotify account passwords are not stored by Paws.
8. Spotify playback naturally requires Premium.

Security note:

Sensitive auth fields (including Spotify tokens, Screenscraper, and RetroAchievements) are stored in `states/authentication.bin` using the Paws auth format (`SRAUTH01`).

- Current format: AES-256-GCM (OpenSSL), 16-byte nonce, authenticated tag, and AAD-bound metadata (version + nonce + payload length).
- Key derivation: device-bound key material derived on-device from hardware/system fingerprint inputs and hashed with SHA-256.
- This is a little bit overkill, but if you wish to use the system, there is no reason not to.

### 📺 Display

Display covers visuals, backgrounds, atmosphere, and text presentation.

Atmosphere features:

- Time of day and season aware background system
- Optional ambience overlays (that can be paried with ambience sounds)
- Stanza editor for dynamic top-right text lines

Current background structure (what Paws is using now):

```
scenes/
  <location>/
    <mood>/
      <season>/                      # optional (supports prefixes like "(i) ")
        morning.png|jpg
        afternoon.png|jpg
        evening.png|jpg
        night.png|jpg
        morning(rain).png|jpg        # optional effect/weather variant, sequential pngs are displayed as gifs.
```

Optional overlay frame paths (tags pair ambience sound with these backgrounds):

```text
scenes/<location>/<mood>/overlays/<tag>/<tag>_001.png
scenes/<location>/overlays/<tag>/<tag>_001.png
overlays/<tag>/<tag>_001.png
```

Alternatively, if you do not wish to associate ambient variations with specific locations, but simply want to add ambient sounds, with or without corresponding overlays:

```text
sounds/ambience/<tag>        #
sounds/ambience/<tag>/<tag>.wav|mp3
sounds/ambience/<tag>/<tag>/overlays/<tag>_001.png

sounds/ambience/it's raining (rain)/overlays/rain_001.png
sounds/ambience/it's raining (rain)/rain.wav
```

Current repo example:

```text
scenes/miyajima/all is still/(iii) autumn/(i) morning.jpg
```

How I set up sync (and how you can change it):

- By default, I map phases to real seasons (`(i) spring`, `(ii) summer`, `(iii) autumn`, `(iv) winter`).
- I map backgrounds to time-of-day (`(i)morning`, `(ii)afternoon`, `(iii)evening`, `(iv)night`).
- With time/season detection enabled, Paws syncs these from your device clock and calendar month.
- You are not locked into this. You can rename folders, use different art, and build your own structure. This is just the default system I use because it keeps everything naturally in sync.

You can use defaults and ignore all of this, or customize deeply.

### 🔊 Sound

Sound controls bells, ambience, and music playback.

Music playback supports local files plus radio streams, Bandcamp, Spotify, and YouTube sources.

Supported sources:

- Local: `.mp3`, `.wav`, `.ogg`, and `.url` stream files
- Radio: internet radio streams via `.url` files (first non-empty line = stream URL)
- Bandcamp: album resolver via `album.bandcamp`, with auto playlist generation (next/previous works)
- Spotify: album resolver via `album.spotify`, with auto playlist generation (next/previous works)
- YouTube: album/video resolver via `album.youtube`; chapters become a playlist when available, and live streams (aka Lofi Girl) are supported (live streams behave as a single stream, not chapter playlist)

How to use it:

1. Create a folder under `music/` (example: `music/<album-name>/`).
2. Choose one source style inside that folder:
   - Local files: drop audio files directly in the folder.
   - Radio stream: create a file like `station.url` and put the station stream URL on the first non-empty line.
   - Bandcamp: create `album.bandcamp` and put the album URL on the first non-empty line.
   - Spotify: create `album.spotify` and put the album URL on the first non-empty line.
   - YouTube: create `album.youtube` and put the video/playlist URL on the first non-empty line.
3. In Paws, switch to that music folder from the main screen and start playback.
4. Use built-in controls to change folder/track, pause, and resume while you focus.

Recommended setup:

1. Use one source file per folder for `album.bandcamp`, `album.spotify`, and `album.youtube`.
2. Put multiple tracks in local folders when you want manual next/previous control.
3. Put multiple `.url` stations in radio folders if you want to hop between stations.

Example:

```
music/
  Focus Set/
    album.bandcamp
  Deep Work/
    album.spotify
  Ambient Coding/
    album.youtube
  Local Jazz/
    01-intro.mp3
    02-loop.wav
  Radio Stations/
    soma.url
    jazz24.url
```

Please be understanding that if you are using Spotify or YouTube, the device may and will take up several seconds to fetch data, prepare chapters, and begin streaming. For some albums, this can take up to 7-8 seconds. Bandcamp, surprisingly, is incredibly fast.

Policy note:

I will not add download support. In fact, I modified the default behavior because it was downloading automatically, so it is unlikely that I will change my mind. Bandcamp integration is for preview/listening only, and I strongly recommend buying the albums you use.

I support background music, as it is central to the experience for most users, but I do not intend for this application to become a full-fledged music player. I am already well beyond the original scope. By tens of thousands of lines of code, in fact.

### 👾 Gameplay

Gameplay covers focus-to-play behavior and runtime constraints.

- A balance rate of `1.0` means every minute of focus earns one minute of playtime to spend in Protocol. I strongly recommend lowering it.
- Game Library scanning caches titles from your ROM folders so simulation suggestions load faster.
- You can manually add focus time and bypass the system, but that goes against the purpose of the system itself. You can also extract time.


## Final Note

If this helps you do even one better session per day, it has done its job.






# Stillroom Keybind Reference


### Main Screen

- `A`: pause/resume active timer run
- `Select`: open Timer Menu.
- `Start` open Settings Menu.
- `Menu` open Protocol Menu
- `Left/Right`: cycle background base (time of the day, if available)
- `Up/Down`: cycle location
- `L1/R1`: previous/next music folder
- `L2/R2`: previous/next track
- `L3`: music on/off.
- `R3`: play/pause current music.
- `Y`: if a session is running, open end-session confirm.
- `X`: toggle meta selector.
  - In meta selector: `Left/Right` change token, `Up/Down` change selected value, `A` random background that matches the highlighted token, `R3` open stanza selector.
- Hold `B` (~`450ms`) or `Power`: toggle HUD visibility.

### Menus

#### Timer Quick Menu (Select Button)
- `1.` Timer
- `2.` Pomodoro
- `3.` Meditation
- `4.` Tasks
- `5.` Routines
- `6.` Booklets

#### Protocol Menu (TrimUI Button)
- `1.` Terminal
- `2.` Balance
- `3.` Simulations
- `4.` Stress Test
- `5.` Protocols
- `6.` Baseline

#### Settings Main Menu (Start)
- `1.` Profile
- `2.` Display
- `3.` Sound
- `4.` Gameplay
- `5.` About
- `6.` Exit App

### Text Entry 

- `Y`: backspace.
- `X`: insert space.
- `R3`: save/confirm text in most text-entry screens.
- `Start`: also saves in some text-entry screens (profile name, some auth fields).

### Extras

- `L3` deletes entries, `R3` creates, saves, or confirms entries.
- `X` and `Y` toggles the current selection in Timer and Meditation.
- Timer/Pomodoro/Meditation pickers: `R3` opens Focus Activity selection.
- Routines: `L2/R2` changes selected day, `Left/Right` changes time of the day.
- Tasks list: `R3` adds item, `L3` deletes selected item, `Y` resets completion marks for current list.

## Credits

<details open> 
<summary><strong>Meditations</strong></summary>
<br>
  
“Mindful Meditations” created by Diana Winston and others for the [UCLA Mindful](https://www.uclahealth.org/uclamindful), ©2011- 2024 The Regents of the University of California (The UC Regents).

Mindful Meditations are licensed under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/).


</details>

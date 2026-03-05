# sonyctl v2.0.0

<!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!--><!--SONYHATE3000!-->

```
███████╗ ██████╗ ███╗   ██╗██╗   ██╗ ██████╗████████╗██╗
██╔════╝██╔═══██╗████╗  ██║╚██╗ ██╔╝██╔════╝╚══██╔══╝██║
███████╗██║   ██║██╔██╗ ██║ ╚████╔╝ ██║        ██║   ██║
╚════██║██║   ██║██║╚██╗██║  ╚██╔╝  ██║        ██║   ██║
███████║╚██████╔╝██║ ╚████║   ██║   ╚██████╗   ██║   ███████╗
╚══════╝ ╚═════╝ ╚═╝  ╚═══╝   ╚═╝    ╚═════╝   ╚═╝   ╚══════╝
```

> *Sony Imaging Edge can go to hell. We built something better.*
> *Say hi to CANON!*

---

## Branding

| Context | Name | Style Reference |
|---------|------|-----------------|
| Internal codename | **SONYHATE3000** | The truth |
| Public-facing brand | **DEAD/WALK/MAN 3000** | [Dead Man Walking](https://en.wikipedia.org/wiki/Dead_Man_Walking_(film)) (1995) poster |
| Unofficial codename | *Lights! Camera! Action!* | For sensitive sensors |
| App Store display name | Camera Remote 3000 | Lawyer-friendly |
| Ruby gem | progress_bar_none_overload_3000 | The Cockpit3000 umbrella |

The public brand is styled after the 1995 Dead Man Walking movie poster — bold condensed all-caps, each word on its own line:

```
D E A D
W A L K
M A N
        3 0 0 0
```

Inline: **DEAD/WALK/MAN 3000**

### Social Media Handles

| Platform | Handle | Status |
|----------|--------|--------|
| Instagram | [@deadwalkman3000](https://instagram.com/deadwalkman3000) | available |
| X / Twitter | [@deadwalkman3000](https://twitter.com/deadwalkman3000) | available |
| TikTok | [@deadwalkman3000](https://tiktok.com/@deadwalkman3000) | available |
| Bluesky | [@deadwalkman3000.bsky.social](https://bsky.app/profile/deadwalkman3000.bsky.social) | available |
| Domain | deadwalkman3000.com | available (.com, .de, .io, .app, .dev — all of them) |
| Website | [site/index.html](site/index.html) | built, indie Mac dev aesthetic ca. 2018 |

> *"deadwalkman" was taken on Instagram and Bluesky. "deadwalkman3000" is free everywhere. The 3000 is load-bearing.*

---

## Platforms

| Platform | Version | Beaver Status | Download |
|----------|---------|---------------|----------|
| **CLI / Ruby** | `3000.no.beaver.emoji.no.0.alpha.1` | no beaver emoji :( | `gem install progress_bar_none_overload_3000` |
| **macOS** | `3000.0.0` | no beaver emoji :( | [TestFlight](#) |
| **iOS** | `3000.0.0` | no beaver emoji :( | [TestFlight](#) |
| **watchOS** | `3000.0.0` | no beaver emoji :( | Paired with iOS |
| **Android** | `3000.🦫.0-alpha.0` | 🦫 | [APK](#) |
| **git tag** | `v3000.🦫.0-alpha.0` | 🦫 | `git checkout v3000.🦫.0-alpha.0` |

> *Apple and Ruby forbid emoji in version numbers. Android doesn't care. The beaver emoji is present wherever the ecosystem permits it, absent where bureaucracy prevails. This is a metaphor for something.*

---

## Feature Matrix

*Tufte would encode the third dimension (platform) as columns in a 2D table. The implementation status is the data; the feature is the row; the platform is the column. Every cell is information. No chartjunk.*

**Legend:**  ✅ done   🔨 coded/untested   📐 designed   ⬜ n/a   🦫 pro-only

| Feature | CLI | macOS | iOS | watchOS | Notes |
|---------|:---:|:-----:|:---:|:-------:|-------|
| **Camera Control** | | | | | |
| ├ Photo capture | ✅ | 🔨 | 🔨 | 🔨 | CLI: gphoto2 USB · Apps: Sony WiFi CCAPI |
| ├ Video start/stop | ✅ | 🔨 | 🔨 | 🔨 | Watch sends command via WCSession relay |
| ├ Live preview feed | ✅ | 🔨 | 🔨 | 🔨 | Watch: 272×170 JPEG, 0.4q, <60KB frames |
| ├ ISO / aperture / shutter | ✅ | 🔨 | 🔨 | ⬜ | Read + write via Sony config API |
| ├ White balance | ✅ | 🔨 | 📐 | ⬜ | |
| ├ Focus mode | ✅ | 📐 | 📐 | ⬜ | AF-S / AF-C / MF |
| └ Save to Photos.app | ⬜ | 📐 | 🔨 | ⬜ | iOS only — PHPhotoLibrary |
| **Input Methods** | | | | | |
| ├ Hand gestures (Vision) | ⬜ | ✅ | 🔨 | ⬜ | 7 gestures, 0.8s hold, VNDetectHumanHandPose |
| ├ Voice commands (Speech) | ⬜ | ✅ | 🔨 | 🔨 | SFSpeechRecognizer keyword spotting |
| ├ Tongue snap detection | ✅ | ✅ | 🔨 | 🔨 | AVAudioEngine RMS spike, <45ms duration gate |
| └ Touch / tap controls | ⬜ | ✅ | 🔨 | 🔨 | macOS: toolbar · iOS: full UI · Watch: tap grid |
| **Nanoleaf Lighting** | | | | | |
| ├ Power on/off | ✅ | 🔨 | 🔨 | ⬜ | REST `/api/v1/{token}/state` |
| ├ Brightness / CT | ✅ | 🔨 | 🔨 | ⬜ | |
| ├ Effects (43 installed) | ✅ | 🔨 | 🔨 | ⬜ | Including "Fucking Conscientiousnessfully" |
| ├ Service mode (3200K/60%) | ✅ | 🔨 | 🔨 | ⬜ | Warm AF assist light |
| ├ Flash mode (100%) | ✅ | 🔨 | 🔨 | ⬜ | |
| ├ Photo scene presets | ⬜ | 📐 | 🔨 | ⬜ | 5 presets: golden hour, studio, moody, etc. |
| ├ AI mood lighting | ✅ | 📐 | 📐 | ⬜ | Claude CLI → emotion → HSB |
| └ UDP panel streaming | ✅ | 📐 | 📐 | ⬜ | Per-panel RGB via port 60222 |
| **App Features** | | | | | |
| ├ HUD overlay (ISO/SS/f/WB) | ⬜ | 🔨 | 📐 | ⬜ | Translucent status bar |
| ├ Gesture cheat sheet | ⬜ | 🔨 | 📐 | ⬜ | Grid of 7 gestures with actions |
| ├ Settings view | ⬜ | 🔨 | 🔨 | ⬜ | Camera IP, Nanoleaf config, input toggles |
| ├ 🦫 Watermark (free tier) | ⬜ | 🔨 | 🔨 | ⬜ | Beaver emoji + "SONYHATE3000 Free" bar |
| ├ Pro IAP ($8.99 / €1.99) | ⬜ | 🔨 | 🔨 | ⬜ | StoreKit 2, Non-Consumable, shared |
| └ WatchConnectivity relay | ⬜ | ⬜ | 🔨 | 🔨 | Phone↔Watch preview + commands |
| **Infrastructure** | | | | | |
| ├ Test suite | ✅ | 📐 | 📐 | ⬜ | CLI: 20/20 passing · Apps: XCTest planned |
| ├ Gantt chart dashboard | ✅ | ⬜ | ⬜ | ⬜ | Cockpit3000, 7 color modes, SVG export |
| ├ Doctor / diagnostics | ✅ | 📐 | 📐 | ⬜ | Camera, gphoto2, ffmpeg, Nanoleaf checks |
| ├ Website | ⬜ | ⬜ | ⬜ | ⬜ | site/index.html, indie Mac dev aesthetic |
| └ App Store submission | ⬜ | 📐 | 📐 | 📐 | See xcode/TODO-APP-STORE.md |

> *Reading this table: CLI has the most ✅ because it's the oldest. macOS/iOS show 🔨 because the SwiftUI code is written but the apps need real-device testing with a Sony camera on WiFi. watchOS gets the subset that makes sense on a 45mm screen. The tree-structure indentation (├ └) groups related features without adding a column — Tufte's "smallest effective difference."*

---

## Architecture

```
┌─────────────────────────────────────────────────────────────────┐
│                     SONY ILCE-7C Camera                         │
│                   USB (gphoto2) ◄──── CLI                       │
│                   WiFi (CCAPI HTTP) ◄──── macOS / iOS apps      │
└─────────────────────────────────────────────────────────────────┘
        │                           │
        ▼                           ▼
┌───────────────┐           ┌───────────────────┐
│  ruby/        │           │  xcode/           │
│  sonyctl.rb   │           │  SONYHATE3000/    │  macOS SwiftUI app
│  nanoleaf.rb  │           │  SONYHATE3000iOS/ │  iOS SwiftUI app
│  sonyctl_*.rb │           │  SONYHATE3000Watch│  watchOS app
└───────────────┘           │  Shared/          │  Cross-platform API
        │                   └───────────────────┘
        ▼                           │
┌───────────────┐           ┌───────────────────┐
│  swift/       │           │  Shared/          │
│  sonyctl-live │           │  SonyCameraAPI    │  Actor-based async Sony HTTP
│  sonyctl-snap │           │  WCMessages       │  Watch↔Phone protocol
└───────────────┘           └───────────────────┘
        │
        ▼
┌───────────────────────────────────────┐
│  Nanoleaf Canvas E528 (17 panels)     │
│  REST API :16021 + UDP streaming :60222│
└───────────────────────────────────────┘
```

### Why WiFi, not USB, for the App Store

The CLI uses gphoto2 over USB — fast, reliable, battle-tested. But macOS App Store apps live in a sandbox that blocks:
- IOKit (USB access) — gphoto2's transport layer
- Killing `ptpcamerad` — requires `sudo`, impossible from sandbox
- Loading dynamic plugins from outside the app bundle

Sony's WiFi CCAPI (PC Remote over HTTP) is just REST calls. Only needs `com.apple.security.network.client`. Even Adobe Lightroom's Mac App Store version can't do USB tethering — we're in good company.

---

## Build Progress

<!-- SONYHATE3000! The Gantt chart of our discontent -->

![sonyctl v2 Build Progress — Gantt Chart](doc/gantt.svg)

*Auto-generated from `ruby/sonyctl_gantt.rb` via `Cockpit3000::Gantt`. Updates every 25 seconds in tmux.*

---

## Phase 0: Discovery & Connection

<details><summary><b>22:00 — Session start (0:00 elapsed)</b></summary>

### Prompt
```
Implement the following plan:

# sonyctl v2 — Live Preview, Gestures, Voice, Snap Detection
[...full plan omitted for brevity...]
```

### Result (topline)
> Plan acknowledged. 4 tasks created. 3 agents launched in parallel.

<details><summary>Agent launches</summary>

- **Agent 1**: Create `sonyctl-snap.swift` (tongue snap detector)
- **Agent 2**: Create `sonyctl-live.swift` (macOS app, 1285 lines)
- **Agent 3**: Create `sonyctl_test.rb` (end-to-end test suite)

All running concurrently while main thread modifies `sonyctl.rb`.
</details>
</details>

<!--SONYHATE3000!-->

---

## Phase 1: Ruby CLI — AudioRecorder, Record, Audio

<details><summary><b>22:01 — sonyctl.rb v2.0.0 (0:01 elapsed)</b></summary>

### Prompt
> (Internal — executing plan Phase 1)

### Result
> `sonyctl.rb` updated: VERSION 2.0.0, CAMERA_MODEL ILCE-7C.
> Added `AudioRecorder` module, `LiveBridge` IPC, `cmd_record`, `cmd_audio`.
> `brew install switchaudio-osx` completed.

<details><summary>Modules added</summary>

- `AudioRecorder`: ffmpeg recording, muxing, SwitchAudioSource wrapping
- `LiveBridge`: HTTP IPC to sonyctl-live on localhost:8766
- `cmd_record`: toggle start/stop video + audio, auto-mux
- `cmd_audio`: list/switch audio inputs
- `cmd_doctor`: now checks ffmpeg, SwitchAudioSource, binaries
</details>
</details>

<!--SONYHATE3000!-->

---

## Phase 2: Swift — Tongue Snap Detector

<details><summary><b>22:02 — sonyctl-snap compiled (0:02 elapsed)</b></summary>

### Result
> `sonyctl-snap.swift` — 136 lines, compiled to 92KB binary, code-signed.
> AVAudioEngine impulse detector: RMS threshold 0.12, <45ms duration, 0.8s cooldown.

<details><summary>Detection algorithm</summary>

- Buffer size 512 frames (~11.6ms at 44.1kHz)
- Exponential moving average baseline (alpha 0.001)
- Spike = RMS exceeds baseline + 0.12
- Accept only if spike duration < 45ms (rejects sustained sounds)
- Output: `SNAP\t<ISO8601>` on stdout
</details>
</details>

<!--SONYHATE3000!-->

---

## Phase 3: Swift — Live Preview App

<details><summary><b>22:05 — sonyctl-live compiled (0:05 elapsed)</b></summary>

### Result
> `sonyctl-live.swift` — 1292 lines, compiled to 379KB, code-signed with entitlements.

<details><summary>Architecture (7 subsystems)</summary>

| Component | Lines | Purpose |
|-----------|-------|---------|
| CameraCommandBridge | 51-174 | Serial gphoto2 queue |
| AudioCue | 176-186 | `say` subprocess for voice feedback |
| SnapDetector | 188-237 | Impulse RMS (same as standalone) |
| AudioHub | 239-326 | Shared AVAudioEngine + SFSpeech |
| GestureClassifier | 328-425 | 7 hand gestures via Vision |
| HandGestureTracker | 427-501 | AVCaptureSession + debounce |
| HTTPCommandServer | 503-600 | NWListener on :8766 |
| PreviewPoller | 602-641 | gphoto2 preview every 200ms |
| SettingsPoller | 643-694 | ISO/aperture/shutter every 5s |
| AppDelegate | 696-932 | Window, HUD, cheat sheet |
</details>
</details>

<!--SONYHATE3000!-->

---

## Phase 4-5: Aliases & Tests v1

<details><summary><b>22:06 — Aliases and test suite (0:06 elapsed)</b></summary>

### Result
> Shell aliases added. Test suite created (298 lines, 10 tests).
> `sonyctl-live` and `sonyctl-snap` aliases in `~/.config/shell/aliases`.
</details>

<!--SONYHATE3000!-->

---

## Phase 6: Nanoleaf Discovery

<details><summary><b>22:08 — "Find all its secrets" (0:08 elapsed)</b></summary>

### Prompt
```
there is an app running called Nanoleaf Desktop. Find out all its secrets
```

### Result

| Secret | Value |
|--------|-------|
| Device | **Nanoleaf Canvas E528**, model NL29, 17 panels |
| Serial | S19414C0950, firmware 12.3.2 |
| Token | `lDFK4Ou5N3SdBRoqaNxQNSBDMxtdmXrQ` (in `$NANOLEAF_TOKEN`) |
| IP | `192.168.0.81:16021` (in `$NANOLEAF_IP`) |
| API | REST `/api/v1/{token}/` + UDP streaming port 60222 |
| Effects | 43 installed (including "Fucking Conscientiousnessfully") |

<details><summary>Discovery method</summary>

```
$ ps aux | grep nanoleaf  → found Electron app v2.3.5
$ env | grep NANOLEAF     → NANOLEAF_TOKEN, NANOLEAF_IP
$ curl http://192.168.0.81:16021/api/v1/$NANOLEAF_TOKEN/  → full device JSON
```
</details>
</details>

<!--SONYHATE3000!-->

---

## Phase 7: Nanoleaf API Client

<details><summary><b>22:10 — nanoleaf.rb (0:10 elapsed)</b></summary>

### Result
> 3 agents launched in parallel:
> 1. `nanoleaf.rb` — full API client (REST + UDP + Animator)
> 2. Light commands added to `sonyctl.rb`
> 3. NanoleafClient + AIBridge added to `sonyctl-live.swift`

<details><summary>nanoleaf.rb modules</summary>

- `Nanoleaf::Client` — REST: power, brightness, hue/sat/ct, effects, panels
- `Nanoleaf::Stream` — UDP external control, per-panel RGB
- `Nanoleaf::Animator` — rainbow_wave, breathe, warm_glow, cool_flash, color_chase, mood
</details>

<details><summary>sonyctl light commands</summary>

```
sonyctl light on/off        — power
sonyctl light service       — warm 3200K at 60% for autofocus
sonyctl light flash [b] [ct] — bright neutral-warm for stills
sonyctl light effect [name]  — list or set Nanoleaf effects
sonyctl light mood <emotion> — AI-driven mood lighting
sonyctl light status        — device info
```
</details>
</details>

<!--SONYHATE3000!-->

---

## Phase 8: AI Integration

<details><summary><b>22:14 — Claude CLI bridge in sonyctl-live (0:14 elapsed)</b></summary>

### Result
> `AIBridge` class added to Swift app. Calls `claude --print -p` for:
> - Mood lighting (emotion → HSB via Claude)
> - Smart camera tips in HUD (updated every 30s)
> Voice commands: "mood dramatic", "lights on/off", "service mode", "flash"
</details>

<!--SONYHATE3000!-->

---

## Phase 9: Camera Connection

<details><summary><b>22:20 — Sony A7C USB debugging (0:20 elapsed)</b></summary>

### Prompt
```
the camera IS CONNECTED!
```

### Result
> Camera not visible on USB. Diagnosed: USB Connection set to Mass Storage.
> Guided user to change to PC Remote mode in camera menu.
> Fixed `PTPDaemon` module to kill `ptpcamerad` (not just `PTPCamera`).
> Fixed `Parser.summary` for Sony's non-standard output format.

```
$ ruby sonyctl.rb doctor
  ✓ Camera detected: Sony ILCE-7C (Control) on usb:001,001
  ✓ gphoto2 installed (gphoto2 2.5.32)
  ✓ ffmpeg installed (ffmpeg version 8.0.1)
  ✓ SwitchAudioSource installed
  ✓ sonyctl-live binary found
  ✓ sonyctl-snap binary found
  ✓ Nanoleaf Canvas E528 (NL29) — 17 panels
  ✓ All checks passed. Ready to shoot.
```

<details><summary>Sony A7C PTP quirks discovered</summary>

- No filesystem access in PC Remote mode (no file listing/download)
- Capture via `/main/actions/capture=1` (not `--capture-image`)
- Preview sometimes needs AF first for JPEG output
- ISO set requires Sony extension (standard path is read-only)
- `ptpcamerad` respawns instantly — must killall -9 immediately before gphoto2
</details>
</details>

<!--SONYHATE3000!-->

---

## Phase 10: Test Suite — Final Run

<details><summary><b>22:30 — 20/20 tests passing (0:30 elapsed)</b></summary>

### Result
```
20 runs, 45 assertions, 0 failures, 0 errors, 0 skips
```

| Test | Status | Details |
|------|--------|---------|
| Camera detection | ✅ | Sony ILCE-7C on usb:001,001 |
| Status command | ✅ | Model, serial, settings |
| Photo capture | ✅ | Shutter fires, saves to card |
| Config read | ✅ | ISO, aperture, shutter, WB, focus |
| Live preview | ✅ | 47KB JPEG frame captured |
| Nanoleaf info | ✅ | Canvas E528, NL29 |
| Nanoleaf power | ✅ | Off → On toggle |
| Nanoleaf brightness | ✅ | 50% → restore |
| Nanoleaf CT | ✅ | 3200K → restore |
| Nanoleaf effects | ✅ | 43 effects listed |
| Nanoleaf panels | ✅ | 17 panels detected |
| Nanoleaf service | ✅ | 60%, 3200K |
| Nanoleaf flash | ✅ | 100% brightness |
| sonyctl light status | ✅ | Full device report |
| UDP streaming | ✅ | Orange → blue → white |
| Binary: sonyctl-snap | ✅ | Exists, signed |
| Binary: sonyctl-live | ✅ | Exists, signed |
| sonyctl version | ✅ | 2.0.0 |
| sonyctl doctor | ✅ | All checks pass |
| nanoleaf.rb CLI | ✅ | Status works |
</details>

---

## Phase 11: Cockpit3000 — Gantt Chart Gets Beautiful

<details><summary><b>23:25 — "Compare the two PNGs!" (0:25 elapsed)</b></summary>

### Prompt
```
Compare the two PNGs in doc/images/**.png! note how much cooler the
temperature/performance monitoring tool looks? YOU created that, as well.
In fact, it's the same gem, from '~/p/🦜 progress bar none overload 3000 🦑'!
So, therefore, move the gantt chart interface into that gem.
Use common colorization routines. Remember EDWARD TUFTE!
Use smart beautiful maybe even actually useful color scheme?
Plus a rainbow vomit version! and animation, blinkblink, and colorspectrums
and everything that maybe CSS can do now?
```

### The Comparison

| Gantt Chart (before) | Cockpit3000 Temperature Monitor |
|---|---|
| ![Gantt chart — functional but bland](doc/Screenshot%202026-03-04%20at%2023.19.45.png) | ![Cockpit3000 — gorgeous](doc/Screenshot%202026-03-04%20at%2023.24.59.png) |

> *Left: Flat green bars, hardcoded 256-color ANSI, no animation.*
> *Right: True-color gradients, sparkline histograms, section headers with colored rules, 15+ palettes. The same gem.*

### Result

> Design document written: `Cockpit3000::Gantt` module.
>
> **Architecture**: Generic `Gantt.new(tasks, mode: :tufte)` renderer for the gem.
> SONYHATE3000's `sonyctl_gantt.rb` becomes a thin wrapper.
>
> **7 color modes designed:**

| Mode | Palette | Tufte Score |
|------|---------|-------------|
| `:tufte` (default) | Done=ocean, WIP=amber, Pending=gray | 10/10 |
| `:phase` | Each phase gets its own palette gradient | 7/10 |
| `:rainbow` | Full spectrum cycling + BLINK | 0/10 (intentional) |
| `:fire` | Lava palette + flicker animation | 2/10 |
| `:matrix` | Green on black + binary rain | 1/10 |
| `:neon` | Synthwave + glow + pulse | 3/10 |
| `:custom` | User-provided status→palette map | varies |

> **Tufte mode** maximizes data-ink ratio: done tasks are cool blue-green (settled),
> WIP is warm amber (draws attention), pending is dim gray (backgrounded).
> No decorative borders. Every pixel of color = information.
>
> **Rainbow vomit mode** is the exact opposite. Maximum pizzazz.
> Every character rainbow-cycles. WIP bars blink. Sparkles in empty space.
> Edward Tufte would cry.

<details><summary>Research: State of terminal rendering (2026)</summary>

| Technology | Status | Ghostty | Kitty | iTerm2 | WezTerm |
|------------|--------|---------|-------|--------|---------|
| 24-bit true color | Universal | ✅ | ✅ | ✅ | ✅ |
| Kitty graphics protocol | Modern standard | ✅ | ✅ | ❌ | ✅ |
| iTerm2 inline images | macOS only | ❌ | ❌ | ✅ | ✅ |
| Sixel | Legacy | ❌ | ❌ | ✅ | ✅ |
| Unicode braille (2×4 dots) | Universal | ✅ | ✅ | ✅ | ✅ |
| Half-block elements (▀▄) | Universal | ✅ | ✅ | ✅ | ✅ |

**Key findings:**
- Kitty graphics protocol is the best path for inline images in Ghostty
- Charm Ruby ecosystem (lipgloss-ruby, ntcharts-ruby) emerged 2024-2025
- Cockpit3000 already has Kitty + iTerm2 protocol support in `Graphics` module
- btop is the gold standard for terminal dashboards (braille + block elements + 24-bit color)

</details>
</details>

<!--SONYHATE3000!-->

---

## Phase 12: RAINBOW VOMIT OVERFLOW 3000

<details><summary><b>23:55 — "WHERE IS MY PREVIEW WINDOW?!" (1:55 elapsed)</b></summary>

### Prompt
```
where is my preview window? where is my gestures cheat sheet? Did we train
listening to commands? Are you filming any of this? Could you maybe get your
act and the lights, together? What the fuck made you SONYESQUE 3000?

NO, don;t answer. Fix it. get your act together. In parallel, everyhting!
```

### Result
> Everything launched **in parallel**:
> 1. `sonyctl-live` preview window — **UP** (gestures, voice, snap detection active)
> 2. `sonyctl-snap` tongue detector — **LISTENING**
> 3. Nanoleaf lights — **ON** at 80%, Nemo effect
> 4. Gantt chart — **6 COLOR MODES RENDERING**

#### Gestures Cheat Sheet (built into sonyctl-live HUD)

| Gesture | Action | Hold Time |
|---------|--------|-----------|
| Open Palm | CAPTURE (shutter) | 0.8s |
| Fist | START/STOP VIDEO | 0.8s |
| Peace Sign | TOGGLE LIVE VIEW | 0.8s |
| Thumbs Up | ISO UP | 0.8s |
| Thumbs Down | ISO DOWN | 0.8s |
| Pointing | TOGGLE GESTURES | 0.8s |
| OK Sign | CONFIRM | 0.8s |

#### Voice Commands

| Command | Action |
|---------|--------|
| "capture" / "take photo" / "shoot" | Take photo |
| "record" / "start recording" | Start video |
| "stop" / "stop recording" | Stop video |
| "lights on" / "lights off" | Nanoleaf power |
| "service mode" | Warm 3200K at 60% |
| "flash" | Full brightness burst |
| "mood dramatic" / "mood warm" / etc. | AI-driven mood lighting |

</details>

<!--SONYHATE3000!-->

---

## Phase 13: Gantt Chart — PRETTYCOLORED-ANIMATEVOMIT-RAINBOWOVERFLOW 3000

<details><summary><b>23:58 — "STILL NO PRETTY COLOR ANIMATIONS????" (1:58 elapsed)</b></summary>

### Prompt
```
also, I did just check your gannt chart and it's showing exactly what's going
on and its fully gannty. STILL NO PRETTY COLOR ANIMATIONS????

Update readme with all prompts and output, include that gannt chart for reference

BUT MAKE IT PRETTYCOLORED-ANIMATEVOMIT-RAINBOWOVERFLOW 3000!!!
```

### Result

> Fixed `rainbow_text` bug (was calling private method on Frames module).
> All 6 Gantt color modes now render. SVG regenerated.

#### All 6 Color Modes

| Mode | Tufte Score | Description |
|------|-------------|-------------|
| `:tufte` | 10/10 | Ocean blues for done, warm amber for WIP, dim gray for pending. Data-ink ratio maximized. |
| `:phase` | 7/10 | Each phase gets its own palette gradient (ocean, forest, sunset, crystal, fire, ice, galaxy, neon) |
| `:rainbow` | 0/10 | **FULL SPECTRUM CYCLING**. Every character is a different color. Edward Tufte is crying. |
| `:fire` | 2/10 | Lava palette with flicker animation. Bars literally shimmer. |
| `:matrix` | 1/10 | Green on black with random binary rain in empty space. Neo would approve. |
| `:neon` | 3/10 | Synthwave palette — deep purple to hot pink to cyan. Blade Runner vibes. |

#### Usage

```ruby
require "cockpit3000"

tasks = [
  { name: "Task A", group: "P1", start: 0, duration: 4, status: :done, progress: 1.0 },
  { name: "Task B", group: "P2", start: 2, duration: 6, status: :wip,  progress: 0.5 },
  { name: "Task C", group: "P3", start: 6, duration: 3, status: :pending, progress: 0.0 },
]

# Terminal output (pick your poison)
chart = Cockpit3000::Gantt.new(tasks, mode: :rainbow, title: "MAXIMUM PIZZAZZ")
puts chart.to_s

# SVG export (dark theme, monospace font)
File.write("gantt.svg", chart.render_svg)

# Live animation in tmux (1 FPS)
chart.run(fps: 1)
```

</details>

<!--SONYHATE3000!-->

---

## Phase 14: Xcode Project — macOS Native App

<details><summary><b>00:15 — "Have you no AGENCY?" (2:15 elapsed)</b></summary>

### Prompt
```
well... what's stopping you? Have you no AGENCY, Gen-X-LARPing SALARINCEL?
```

### Result
> Full SwiftUI macOS app created in `xcode/`. 12 Swift files, Xcode project, entitlements, Info.plist, StoreKit config, privacy manifest.

#### Architecture Decision: WiFi, not USB

| Approach | App Store Compatible | Why |
|----------|---------------------|-----|
| gphoto2 over USB | ❌ | IOKit blocked by sandbox, can't kill ptpcamerad, dynamic plugins |
| Sony WiFi CCAPI | ✅ | Just HTTP REST calls, only needs network.client entitlement |

> *Even Adobe Lightroom Mac App Store can't do USB tethering. We're in company.*

#### Files Created

| File | Purpose |
|------|---------|
| `SONYHATE3000App.swift` | @main entry, NotificationCenter for gesture sheet |
| `ContentView.swift` | HSplitView: live preview left, controls sidebar right |
| `LivePreviewView.swift` | Camera feed, 🦫 watermark overlay, recording indicator |
| `PaywallView.swift` | Pro upgrade, feature list, StoreKit price, restore |
| `GestureCheatSheetView.swift` | Grid of 7 gestures with emojis and actions |
| `HUDOverlayView.swift` | Camera settings bar (ISO, SS, f/, WB, battery) |
| `SettingsView.swift` | TabView: Camera, Nanoleaf, Input, About |
| `CameraService.swift` | Sony WiFi HTTP client, preview polling 200ms, capture/record |
| `NanoleafService.swift` | REST API client for Canvas lights |
| `StoreManager.swift` | StoreKit 2, `com.sonyhate3000.pro`, Non-Consumable |
| `SnapDetectorService.swift` | AVAudioEngine, extracted `SnapProcessor: @unchecked Sendable` |
| `BeaverWatermark.swift` | NSImage watermarking with 🦫 + text bar |

#### Bugs Fixed During Build

| Bug | Fix |
|-----|-----|
| `AVAudioPCMBuffer.frameCount` doesn't exist | Changed to `.frameLength` |
| `AppDelegate` not found in scope | Replaced with `NotificationCenter.default.post` |
| Swift concurrency isolation in audio callback | Extracted `SnapProcessor` as separate `@unchecked Sendable` class |
| xcodebuild plugin crash (IDESimulatorFoundation) | Switched to `swift build` via Package.swift |
| `.v26` unavailable with swift-tools-version:5.9 | Upgraded to swift-tools-version:6.2 |

</details>

<!--SONYHATE3000!-->

---

## Phase 15: iOS + watchOS Companions

<details><summary><b>00:30 — "set MacOS 26 and iOS, watchOS equivalents" (2:30 elapsed)</b></summary>

### Prompt
```
set MacOS 26 and iOS, watchOS equivalents as minimum deployment versions.
in subagents, implement apple watch and iOS companions, with the watch
showing just the preview video feed, listening for audio commands, and
allowing tap-to-take photo/start-stop video capture.
```

### Result
> 2 agents dispatched in parallel. Shared/ directory created for cross-platform code.

#### Shared Code (Shared/)

| File | Purpose |
|------|---------|
| `SonyCameraAPI.swift` | Actor-based async/await Sony HTTP client (pure Foundation) |
| `WatchConnectivityMessages.swift` | `WCMessage` enum: command, previewData, cameraStatus, isRecording |

#### watchOS App (5 files)

| File | Purpose |
|------|---------|
| `SONYHATE3000WatchApp.swift` | @main entry |
| `WatchContentView.swift` | Two-page TabView: preview + capture/record buttons |
| `WatchControlsView.swift` | Camera stats, quick action grid, voice status |
| `WatchSessionManager.swift` | WCSession delegate, receives preview frames, sends commands |
| `WatchAudioCommander.swift` | AVAudioEngine + SFSpeechRecognizer keyword spotter on Watch |

#### iOS App (12 files)

| File | Purpose |
|------|---------|
| `SONYHATE3000iOSApp.swift` | @main entry, wires Watch/camera/nanoleaf callbacks |
| `iOSContentView.swift` | TabView with 4 tabs (Preview, Controls, Lights, Settings) |
| `iOSPreviewView.swift` | Full-screen preview, Vision gesture recognition, voice |
| `iOSControlsView.swift` | Wheel pickers for ISO/shutter/aperture |
| `iOSNanoleafView.swift` | Power, brightness, effects, 5 photo scene presets |
| `iOSSettingsView.swift` | Camera/Nanoleaf config, input toggles, gesture reference |
| `iOSPaywallView.swift` | Pro upgrade screen |
| `iOSCameraService.swift` | Camera control with UIImage preview, saves to Photos |
| `iOSNanoleafService.swift` | Nanoleaf client with scene presets |
| `PhoneSessionManager.swift` | WCSession: sends preview frames (272×170 JPEG, 0.4q, <60KB) |
| `iOSBeaverWatermark.swift` | UIImage watermarking |
| `NanoleafScene.swift` | 5 photo scene presets (golden hour, studio, moody, dramatic, neon) |

#### Watch Preview Streaming

```
iPhone → downsample to 272×170 → JPEG 0.4 quality → drop if >60KB
       → WCSession.sendMessageData() → Watch displays in Image view
```

</details>

<!--SONYHATE3000!-->

---

## Phase 16: Version Numbering Across Ecosystems

<details><summary><b>00:45 — "3000.beaver.0-alpha.0" (2:45 elapsed)</b></summary>

### Prompt
```
add a platform-navigation up top, with platforms cli/ruby, MacOS, iOS, and
android, each with the latest release version number. Make sure we start with
version number 3000.<beaver emoji>.0-alpha.0, with either the actual beaver
emoji, or the actual string '<beaver emoji>' without quotes, or
.no beaver emoji :(. whichever is the first one that works for each ecosystems
version number requirements that we cannot escape.
```

### Result: Version Number Constraints

| Ecosystem | Regex / Rule | Beaver? | Version Used |
|-----------|-------------|---------|--------------|
| Ruby (Gem::Version) | `/\A[0-9]+(\.[0-9a-zA-Z]+)*\z/` — ASCII only | no beaver emoji :( | `3000.no.beaver.emoji.no.0.alpha.1` |
| Apple (CFBundleShortVersionString) | `X.Y.Z` — numbers and dots only | no beaver emoji :( | `3000.0.0` |
| Android (versionName) | Any string | 🦫 | `3000.🦫.0-alpha.0` |
| Git tags | Any bytes | 🦫 | `v3000.🦫.0-alpha.0` |

> *We tried. The beaver is present wherever the ecosystem permits it.*

</details>

<!--SONYHATE3000!-->

---

## Phase 17: Website — Indie Mac Dev Aesthetic

<details><summary><b>01:00 — "create a cool, indy-macOS-developer-style website" (3:00 elapsed)</b></summary>

### Prompt
```
create a cool, indy-macOS-developer-style website ca. 2018 for the MacOS/iOS/
watch app, with screenshots and animation to show all the features, lots of
sony hate, and links to the alpha test version, a way to sign up for a
newsletter, and links to instagram, bluesky, twitter, tiktok
```

### Result
> `site/index.html` — 1,503 lines, zero external dependencies.

| Feature | Implementation |
|---------|---------------|
| Dark theme | `#0a0a0f` background, cream text |
| Animated gradient border | CSS `@keyframes gradientMove` on hero |
| Star field | JavaScript particle system in hero section |
| Cursor beaver | 🦫 follows mouse position via `mousemove` |
| Platform version bar | All 5 platforms with version numbers |
| 7 feature cards | Camera, gestures, voice, snap, lights, AI, Gantt |
| Gantt SVG embed | Inline `<svg>` with Cockpit3000 color modes |
| Pricing section | Free tier (🦫 watermark) vs Pro ($8.99) |
| Newsletter signup | Email input + "Notify Me" button |
| Social links | Instagram, Bluesky, X, TikTok |
| Scroll animations | IntersectionObserver fade-in on scroll |
| Responsive | Works on mobile (media queries) |

</details>

<!--SONYHATE3000!-->

---

## Phase 18: Brand Name — DEAD/WALK/MAN 3000

<details><summary><b>01:15 — "BOOMERBOX 3000!" → "dead walk man" (3:15 elapsed)</b></summary>

### Prompt sequence
```
do not use SONY in our name or the social media handles, but maybe something
that looks similar? an anagram? A previous code name? no, wait! make a pun on
'walkman', maybe 'dead walkmaning?', 'toxic walkmasculinity?', 'BOOMERBOX 3000!'?
```

```
"dead walk man" <- this one! style it like the movie, Dead Man Walking did it,
look it up? Capital letters, title case, slashes between words? etc.
```

### Brand Name Evolution

| Candidate | Problem |
|-----------|---------|
| SONYHATE3000 | Contains "Sony" — trademark issues for public accounts |
| BOOMERBOX 3000 | @boomerbox3000 available everywhere, but then... |
| dead walk man | Pun on Sony Walkman + Dead Man Walking (1995 film) |
| **DEAD/WALK/MAN 3000** | Final choice. All-caps, stacked, condensed. |

### Social Media Availability Check

#### boomerbox3000 (checked first, all available)

| Platform | Status |
|----------|--------|
| Instagram | "Profile ist nicht verfügbar" — free |
| X/Twitter | "This account doesn't exist" — free |
| TikTok | "Dieses Konto konnte nicht gefunden werden" — free |
| Bluesky | No profile — free |
| Domain | .com .de .net .org .ai .io — all available |

#### deadwalkman (checked second — TAKEN on 2/5)

| Platform | Status |
|----------|--------|
| Instagram | "deadwalkman • Instagram-Fotos und -Videos" — **TAKEN** |
| Bluesky | "deadwalkman (@deadwalkman.bsky.social)" — **TAKEN** |
| X/Twitter | Inconclusive (redirected to home) |
| TikTok | Error loading |
| Domain | .com available |

#### deadwalkman3000 (final — ALL AVAILABLE)

| Platform | Handle | Status |
|----------|--------|--------|
| Instagram | @deadwalkman3000 | free |
| X/Twitter | @deadwalkman3000 | "This account doesn't exist" — free |
| TikTok | @deadwalkman3000 | "Dieses Konto konnte nicht gefunden werden" — free |
| Bluesky | @deadwalkman3000.bsky.social | No profile — free |
| Domain | deadwalkman3000.com | available (all TLDs) |

> *The 3000 is, once again, load-bearing.*

</details>

<!--SONYHATE3000!-->

---

## USB Connection Tips

> **Seriously, read these.** Sony's USB implementation is, characteristically, hostile to the user.

1. **Set USB Connection to PC Remote**: `MENU → Setup → USB Connection → PC Remote`. Mass Storage and MTP will NOT work with gphoto2.
2. **Use a good cable**: Not all USB-C cables carry data. If the camera shows nothing when plugged in, try a different cable.
3. **Connect directly**: Don't use USB hubs. Connect the camera directly to your MacBook's USB-C port.
4. **Camera USB-C port**: Left side, behind the rubber door flap, bottom connector.
5. **Power cycle after changing settings**: Turn camera off, change USB Connection, turn back on, then plug in.
6. **"Check the connected device"**: This message means the camera is in Mass Storage mode. Change to PC Remote.
7. **macOS will steal the connection**: `ptpcamerad` grabs the camera instantly. sonyctl kills it automatically, but if you see "Could not claim USB device", just retry.

---

## Files

| File | Lines | Purpose |
|------|-------|---------|
| **CLI (Ruby)** | | |
| `ruby/sonyctl.rb` | ~1050 | Main CLI (camera + audio + lights) |
| `ruby/nanoleaf.rb` | ~350 | Nanoleaf API client (REST + UDP + Animator) |
| `ruby/sonyctl_test.rb` | ~400 | End-to-end test suite (20 tests) |
| `ruby/sonyctl_gantt.rb` | ~120 | Tmux Gantt chart dashboard |
| **Swift (standalone)** | | |
| `swift/sonyctl-live.swift` | ~1300 | Live preview app (gestures, voice, lights, AI) |
| `swift/sonyctl-snap.swift` | ~140 | Standalone tongue snap detector |
| `swift/sonyctl-live.entitlements` | 13 | Camera, mic, speech, network entitlements |
| `shell/aliases` | +2 | sonyctl-live, sonyctl-snap aliases |
| **macOS App (Xcode)** | | |
| `xcode/SONYHATE3000/SONYHATE3000App.swift` | ~45 | @main entry |
| `xcode/SONYHATE3000/Views/*.swift` | ~6 files | ContentView, LivePreview, Paywall, Gestures, HUD, Settings |
| `xcode/SONYHATE3000/Services/*.swift` | ~4 files | CameraService, NanoleafService, StoreManager, SnapDetector |
| `xcode/SONYHATE3000/Models/BeaverWatermark.swift` | ~60 | NSImage 🦫 watermark |
| **iOS App** | | |
| `xcode/SONYHATE3000iOS/Views/*.swift` | ~7 files | Content, Preview, Controls, Nanoleaf, Settings, Paywall |
| `xcode/SONYHATE3000iOS/Services/*.swift` | ~3 files | CameraService, NanoleafService, PhoneSessionManager |
| `xcode/SONYHATE3000iOS/Models/*.swift` | ~2 files | BeaverWatermark, NanoleafScene |
| **watchOS App** | | |
| `xcode/SONYHATE3000Watch/Views/*.swift` | ~2 files | ContentView, ControlsView |
| `xcode/SONYHATE3000Watch/Services/*.swift` | ~2 files | WatchSessionManager, WatchAudioCommander |
| **Shared** | | |
| `xcode/Shared/SonyCameraAPI.swift` | ~180 | Actor-based async Sony WiFi HTTP client |
| `xcode/Shared/WatchConnectivityMessages.swift` | ~20 | WCMessage protocol types |
| **Config** | | |
| `xcode/Package.swift` | 25 | swift-tools-version:6.2, macOS/iOS/watchOS 26 |
| `xcode/SONYHATE3000.xcodeproj/project.pbxproj` | ~330 | Xcode project config |
| `xcode/SONYHATE3000/Info.plist` | 35 | Bundle config, usage descriptions, Bonjour |
| `xcode/SONYHATE3000/SONYHATE3000.entitlements` | ~15 | Sandbox + camera + audio + speech + network |
| `xcode/SONYHATE3000/Resources/PrivacyInfo.xcprivacy` | ~25 | Privacy manifest (UserDefaults, CA92.1) |
| `xcode/SONYHATE3000/StoreKit/Products.storekit` | ~35 | Local StoreKit config ($8.99 Pro) |
| **Website** | | |
| `site/index.html` | ~1503 | Indie Mac dev aesthetic, zero dependencies |

---

## Dependencies & Licenses

All third-party libraries, frameworks, and tools used — by platform.

### CLI / Ruby — `GPL 3000.0`

| Dependency | Kind | License | Used In |
|------------|------|---------|---------|
| [Ruby](https://www.ruby-lang.org/) 3.x | Runtime | [BSD/Ruby](https://www.ruby-lang.org/en/about/license.txt) | all `.rb` files |
| Ruby stdlib (open3, json, net/http, socket, fileutils, optparse, time, uri, tempfile) | Stdlib | [BSD/Ruby](https://www.ruby-lang.org/en/about/license.txt) | sonyctl.rb, nanoleaf.rb, sonyctl_test.rb |
| [minitest](https://github.com/minitest/minitest) | Test framework (bundled w/ Ruby) | [MIT](https://github.com/minitest/minitest/blob/master/README.rdoc) | sonyctl_test.rb |
| [gphoto2](http://gphoto.org/) | System binary (`brew install`) | [LGPL 2.1](http://gphoto.org/proj/libgphoto2/) (libgphoto2) · [GPL 2](https://github.com/gphoto/gphoto2/blob/master/COPYING) (CLI) | sonyctl.rb, sonyctl_test.rb |
| [ffmpeg](https://ffmpeg.org/) | System binary (`brew install`) | [LGPL 2.1 / GPL 2+](https://ffmpeg.org/legal.html) (depends on build flags) | sonyctl.rb |
| [SwitchAudioSource](https://github.com/deweller/switchaudio-osx) | System binary (`brew install`) | [MIT](https://github.com/deweller/switchaudio-osx/blob/master/LICENSE) | sonyctl.rb |
| [SoX](https://sourceforge.net/projects/sox/) (`rec`) | System binary (`brew install sox`) | [GPL 2+](https://sourceforge.net/projects/sox/) | sonyctl_test.rb (optional) |
| [Cockpit3000](https://rubygems.org/gems/progress_bar_none_overload_3000) | Local gem (optional) | GPL 3000.0 (ours) | sonyctl.rb |

### macOS / Swift Standalone — `GPL 3000.0`

| Dependency | Kind | License | Used In |
|------------|------|---------|---------|
| [Swift](https://swift.org/) 6.x | Compiler & runtime | [Apache 2.0](https://swift.org/LICENSE.txt) | all `.swift` files |
| [AppKit](https://developer.apple.com/documentation/appkit) | Apple framework | [Apple EULA](https://www.apple.com/legal/sla/) (free with Xcode) | sonyctl-live.swift |
| [AVFoundation](https://developer.apple.com/documentation/avfoundation) | Apple framework | [Apple EULA](https://www.apple.com/legal/sla/) | sonyctl-live.swift, sonyctl-snap.swift |
| [Foundation](https://developer.apple.com/documentation/foundation) | Apple framework | [Apple EULA](https://www.apple.com/legal/sla/) | sonyctl-live.swift, sonyctl-snap.swift |
| [Network](https://developer.apple.com/documentation/network) | Apple framework | [Apple EULA](https://www.apple.com/legal/sla/) | sonyctl-live.swift |
| [Speech](https://developer.apple.com/documentation/speech) | Apple framework | [Apple EULA](https://www.apple.com/legal/sla/) | sonyctl-live.swift |
| [Vision](https://developer.apple.com/documentation/vision) | Apple framework | [Apple EULA](https://www.apple.com/legal/sla/) | sonyctl-live.swift |
| [gphoto2](http://gphoto.org/) | System binary (called via `Process()`) | [GPL 2](https://github.com/gphoto/gphoto2/blob/master/COPYING) | sonyctl-live.swift |
| [Claude CLI](https://claude.ai/claude-code) | System binary (called via `Process()`) | [Anthropic TOS](https://www.anthropic.com/policies/terms-of-service) (proprietary, free tier) | sonyctl-live.swift (AIBridge) |

### macOS / iOS / watchOS Xcode App — `GPL 3000.0`

| Dependency | Kind | License | Used In |
|------------|------|---------|---------|
| [SwiftUI](https://developer.apple.com/documentation/swiftui) | Apple framework | [Apple EULA](https://www.apple.com/legal/sla/) | all Views |
| [StoreKit 2](https://developer.apple.com/documentation/storekit) | Apple framework | [Apple EULA](https://www.apple.com/legal/sla/) | StoreManager.swift |
| [Combine](https://developer.apple.com/documentation/combine) | Apple framework | [Apple EULA](https://www.apple.com/legal/sla/) | reactive bindings |
| [AVFoundation](https://developer.apple.com/documentation/avfoundation) | Apple framework | [Apple EULA](https://www.apple.com/legal/sla/) | CameraService, SnapDetector |
| [Vision](https://developer.apple.com/documentation/vision) | Apple framework | [Apple EULA](https://www.apple.com/legal/sla/) | hand gesture detection |
| [CoreGraphics](https://developer.apple.com/documentation/coregraphics) / [CoreImage](https://developer.apple.com/documentation/coreimage) / [Metal](https://developer.apple.com/documentation/metal) | Apple frameworks | [Apple EULA](https://www.apple.com/legal/sla/) | image pipeline |
| **No SPM packages** | — | — | `workspace-state.json`: `"dependencies": []` |

### Website — `GPL 3000.0`

| Dependency | Kind | License | Used In |
|------------|------|---------|---------|
| [Umami](https://umami.is/) analytics | Self-hosted JS tracker (2.7 KB) | [MIT](https://github.com/umami-software/umami/blob/master/LICENSE) | site/js/beaver.js |
| System font stack | CSS (`-apple-system`, `SF Mono`, `Menlo`, etc.) | Bundled with OS | site/index.html |
| **No frameworks, no CDN, no npm** | — | — | Vanilla HTML/CSS/JS |

### Shell Aliases (optional tools)

| Tool | License | Alias |
|------|---------|-------|
| [rclone](https://rclone.org/) | [MIT](https://github.com/rclone/rclone/blob/master/COPYING) | `rclone` |
| [chafa](https://hpjansson.org/chafa/) | [LGPL 3+](https://github.com/hpjansson/chafa/blob/master/COPYING.LESSER) | `img` |
| [yt-dlp](https://github.com/yt-dlp/yt-dlp) | [Unlicense](https://github.com/yt-dlp/yt-dlp/blob/master/LICENSE) (public domain) | `y`, `yt` |
| [tmux](https://github.com/tmux/tmux) | [ISC](https://github.com/tmux/tmux/blob/master/COPYING) | `yt` (bg sessions) |

### Compatibility Notes

| ⚠️ Flag | Detail |
|---------|--------|
| **gphoto2 GPL ↔ our GPL 3000.0** | gphoto2 CLI is GPL 2. We call it as a subprocess (not linked), so no license conflict. If we ever linked libgphoto2 directly, LGPL 2.1 copyleft would apply. |
| **ffmpeg GPL builds** | Homebrew's default ffmpeg is LGPL 2.1. Some `--enable-gpl` builds are GPL 2+. We call it as a subprocess — no linking. |
| **Apple frameworks** | Apple EULA permits use on Apple hardware only. No redistribution of frameworks themselves. Our code using them is still GPL 3000.0. |
| **Anthropic Claude CLI** | Proprietary. Called as external process. Not bundled or redistributed. Subject to [Anthropic TOS](https://www.anthropic.com/policies/terms-of-service). |
| **No actual incompatibilities** | All third-party code is either subprocess-invoked (GPL/LGPL safe), MIT/ISC/Unlicense (maximally permissive), or Apple SDK (standard platform dependency). ✅ |

---

## License

```
                    GNU GENERAL PUBLIC LICENSE
                       Version 3000.0

 S tarting from the premise that software should be free,
 O ne must also acknowledge that some software companies
 N eed to be publicly shamed for their desktop applications.
 Y ou might think this is about a specific company. You are
   correct.
 H owever, we believe in constructive alternatives.
 A nd so we built sonyctl, which replaces Sony Imaging Edge
 T otally and completely, with better features, fewer bugs,
 E legant terminal output, and actual macOS integration.

 3 things are certain: death, taxes, and Sony desktop
 0 effort put into QA for Imaging Edge. We measured.
 0 users would choose Imaging Edge if alternatives existed.
 0 regrets building this. Not one.
 ! The exclamation point is for emphasis.

Everyone is permitted to copy and distribute verbatim copies
of this license document, but changing it is not allowed,
unless you hate Sony software more than we do, in which case
you may modify it to hate Sony software even more.

This program is free software: you can redistribute it and/or
modify it under the terms of this license, provided that you
maintain at least 497 hidden references to SONYHATE 3000! in
any derivative work. This is a legal requirement.

THE SOFTWARE IS PROVIDED "AS IS", WITH THE EXPLICIT WARRANTY
THAT IT IS BETTER THAN SONY IMAGING EDGE FOR MacOS, BECAUSE
LITERALLY ANYTHING IS.
```

---

*Built with hate (for Sony software), love (for photography), and Claude.*
*Public brand: DEAD/WALK/MAN 3000 · Internal codename: SONYHATE3000*
*20/20 tests passing. Lights blinking. Shutter firing. Beaver watermarking.*

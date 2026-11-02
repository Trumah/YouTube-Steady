YouTube Steady public distribution

The complete corresponding source is in YouTube-Steady-2.1.2-source.zip.
Extract that archive for the extension source, build scripts, translations,
native reference tests and public validation reports. The GPL license and
third-party notices are included in both packages.

YouTube Steady 2.1.2

Real-time, translation-only video stabilization inside the YouTube player.
The DePan / FFTW WebAssembly core runs on your device. YouTube still controls
audio, seeking, speed and fullscreen. No preliminary download or conversion.

Install / share
  The YouTube-Steady-2.1.2.zip archive contains the extension itself.
  Extract it into one folder. In desktop Chrome, open Extensions > Manage
  extensions, enable Developer mode, choose Load unpacked, and select that
  folder. Keep the folder, including the .wasm file and _locales directory.
  This is an unpacked extension package, not a Chrome Web Store listing.
  When updating an existing unpacked copy, replace its files, reload the
  extension, then refresh already-open YouTube pages.

Use
  Open a regular www.youtube.com/watch video and select Stabilize in the
  player. Enable or disable stabilization there, without a separate shortcut.
  Edit the numeric fields and choose Apply settings or press Enter.
  Reset defaults restores the original 1.06x profile and keeps your language.
  Settings are saved in this browser profile, including across page reloads.
  Copying the extension to another computer does not copy browser settings.

Language and numbers
  Automatic prefers the browser UI language, then supported language
  preferences, with English as the final fallback. You can override it in
  the player or the extension popup. Languages use their own written names.
  Included: English, Traditional Chinese, Simplified Chinese, Japanese,
  Korean, Spanish, Brazilian Portuguese, French, German, Russian, Arabic,
  and Hindi. Arabic uses a right-to-left layout. Language changes preserve
  the current motion state and numeric drafts that have not been applied.
  Automatic mode retains regional number conventions where available.
  Inputs accept a decimal point or comma and Arabic, Persian, Devanagari
  and fullwidth digits. Do not use thousands separators in numeric inputs.
  Up/Down steps a numeric field; Shift+Up/Down uses ten steps.
  Escape closes the panel and returns focus to its button.

Default parameters (source-pixel units)
  Zoom             1.06    1.00 keeps the full frame; edges may expose black.
  cutoff           1.25    Lower: stronger smoothing, slower camera following.
  damping          1.0     Response / rebound; start with small changes.
  dxmax / dymax    128     Soft compensation limits; 0 locks that axis.
  winx / winy      512     Centered analysis window, bounded by source size.
  estimate.dx/dy   192     Search range, capped below half the active window.
  trust            4      Higher rejects more uncertain motion estimates.
  stab             1      Confidence penalty for large estimated motion.
  subpixel         1      Bilinear interpolation; 0 uses nearest neighbor.
  Advanced controls retain native parameter names to help reproduce profiles.

Compatibility and limits
  Desktop Chrome 120+ is required. Tested on Chrome 156 / Windows. Other
  Chromium browsers are not separately qualified. Normal 24-30 fps playback
  at 1x is the main validated use case. Higher speeds, 48/60 fps and 4K depend
  on the device and stream; reducing the analysis window is not guaranteed
  to improve cadence. The earlier 1080p/24 at 2x test did not reach all 48
  required output frames per second. This UI release keeps that same core.
  The current synthetic 1080p/30 comparison produced 29.2 fps in 2.1 and
  29.4 fps in 2.0, with dropped frames in both versions and the original
  player. The strict cadence checks did not pass. See
  validation/public-validation.json in the source package for measured
  results and their scope; these are not guarantees for every device.
  Rotation, zoom, rolling-shutter distortion and large foreground movement
  cannot always be fixed by global translation. Exposed edges are black.
  Protected or unreadable video falls back to the original. PiP / Cast uses
  the original video. HDR output is not calibrated. If processing stops,
  Apply settings retries without changing the chosen parameters.

Privacy / source
  Storage is the only API permission; the content script runs on YouTube.
  No analytics, remote translation services, downloaded code or web fonts.
  The installable ZIP excludes development pages and local browser records.
  The matching -source.zip supplies corresponding source, FFTW source,
  synthetic reference data, fixture-generation scripts, build scripts and
  public validation information.
  See README-build.txt to build or test; TRANSLATING.txt to add a language.
  GNU GPL version 2 or later. See LICENSE.txt and NOTICE.txt.

Optional one-time support and free publication
  The owner-approved public receiver is https://paypal.me/TrumanSun
  (Sun Truman, @TrumanSun), verified on the public PayPal.Me profile.
  Tips are optional and use an amount chosen by the supporter; no subscription
  or automatic renewal is created. Payment fees and regional availability
  still apply. No real payment was made as part of release verification.
  The public website remembers its language preference; the hosting provider
  may keep ordinary access logs. The extension adds no payment SDK or extra
  API permissions. See PUBLISHING.txt for setup and free GitHub distribution.
  This is a preview release. Public profile/link checks do not verify account
  eligibility, completion of a payment or withdrawal to a bank account.

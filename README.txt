Video Stabilizer public distribution

The complete corresponding source is in Video-Stabilizer-2.9.6-source.zip.
Extract that archive for the extension source, build scripts, translations,
native reference tests and public validation reports. The GPL license and
third-party notices are included in both packages.

Video Stabilizer 2.9.6

2.9.6 sustained playback reminders (local update)
  After about five effective seconds of sustained trouble, the player icon
  gains an amber border and ! symbol, with one four-second notice per incident.
  Open the panel for measured output/source fps and evidence-based advice:
  processing pressure, source frame drops, buffering, or an undetermined cause.
  Processing advice offers Q (sampling size) and lower YouTube resolution.
  The buttons only locate Q or Performance; values change only by your action.
  Ten healthy seconds clear the warning. Startup, seeking, pauses, ads and
  hidden pages are excluded; callback misses recovered by the watchdog do
  not alone trigger a warning. There is no flashing animation.
  All 12 languages include localized numbers, accessible status messages
  and right-to-left layout. Current settings and saved profiles are retained.

2.9.5 independent frame cadence (local update)
  A native-frame watchdog fills gaps in video callback delivery. Repeated
  timestamps are closed before analysis, with one job and one timer at most.
  Pause, seek, hidden pages, errors and disable stop both scheduling paths.
  Normal canvas compositing presents completed output frames. User settings
  and the native processing core are preserved. Historical notes follow.

2.9.4 last applied settings (local update)
  Apply saves confirmed settings for subsequent videos, new tabs, reloads and
  browser restarts. My default is a separate preset for manual restoration.
  Enable stays immediate and is remembered. Closing cancels only drafts.
  Read/save errors remain visible with Retry; failed saves keep active values.
  First upgrade uses the existing personal default until the first Apply.
  Older versions did not persist Apply-only values. Historical notes follow.

2.9.3 packaged core loading
  Browser startup compiles unchanged local WASM bytes delivered by Chrome as
  a content script. No page-to-extension WASM request is made. Missing or
  corrupt data still restores original playback and reports an error.
  Update every file in the existing folder, reload the extension, then refresh
  existing YouTube pages. Processing defaults and current schema9/format2
  profiles are retained; older processing schemas use the new system defaults.
  Use Video-Stabilizer-2.9.3.zip and Video-Stabilizer-2.9.3-source.zip.
  See validation/embedded-core-browser-2.9.3.json for evidence and limitations.
  On 2026-11-05, the user reported no further Chrome Errors and normal
  stabilization with 2.9.3, and authorized public distribution. This is a
  user-reported real-use check; Edge remains unvalidated.



2.9.2 product rename (local release, not published)
  Video Stabilizer is the new product name; earlier releases used YouTube Steady.
  All features remain free, with optional one-time support and no subscription.
  Target: YouTube in desktop Google Chrome. Microsoft Edge is not validated.
  Processing, defaults, icon artwork and saved-profile identifiers are retained.
  Update the existing installed folder to keep its extension identity and data.
  Install: Video-Stabilizer-2.9.2.zip; source: Video-Stabilizer-2.9.2-source.zip.
  The historical repository URL is retained; no public release was changed.
  Validation: validation/rename-browser-2.9.2.json. Earlier notes follow.

2.9.1 staged presets and confirmed-only saving
  Apply is available only while the form differs from the applied settings.
  System defaults and Restore my default only fill the form, including Enable;
  Apply is required to use them. Closing, Escape or the entry toggle discards
  all unapplied processing edits and keeps the last explicitly applied values.
  Save as my default is beside Apply and enabled only when no draft remains.
  It saves the confirmed values without applying or restarting processing.
  Direct Enable, language and icon changes remain immediate. Processing errors
  have a separate Retry button. Defaults and native calculations are unchanged.
  See validation/apply-confirm-browser-2.9.1.json. Older notes are historical.

2.9.0 one personal default and compact controls
  Enable switches stabilization on/off. Show regions and Restore my default
  share a row; C and cutoff remain common, with the other fields in Advanced.
  Apply changes this viewing only. Save as my default validates and applies
  the current form, then saves one profile for later videos. Closing, Escape
  or closing through the player icon discards unapplied edits. Enable,
  language and icon preferences still take effect immediately.
  There is no comparison button, local undo, previous-default restore,
  Cancel edits button or My default section. System defaults remain available.
  The current schema9/format2 personal profile is retained. Older backups are
  ignored, and the next save replaces the record with one profile only.
  Normal explanations use tooltips and accessible descriptions; bounds and
  capacity warnings remain visible. Detailed readings are under Performance.
  Defaults and the native core are unchanged from2.8.1. See
  validation/ui-simplify-browser-2.9.0.json. Version notes below are historical.

2.8.1 control order and general defaults
  Common: Compensation C%, cutoff Hz, My default.
  Advanced: damping, detection mode, R%, Q%, center priority, S%, trust,
  large-motion penalty, subpixel interpolation, zoom, player icon, language.
  Defaults: C15%, cutoff0.5Hz, damping0.3, central region only, R85%, Q30%,
  center priority off, regional S30%, trust4, penalty1, bilinear, zoom1.00,
  player icon shown and automatic browser language. Priority stays visible
  but disabled for central-only mode; it remains available in multi-region modes.
  Existing schema9/format2 personal profiles and backups stay unchanged.
  Restore general defaults adopts these values for this viewing; Save as my
  default explicitly makes them the baseline for later videos. The native core,
  five-second preview and recovery protections are unchanged.
  Verification: validation/ui-defaults-browser-2.8.1.json.
  The version-specific sections below are historical notes.

2.8.0 regional search and seconds
  Search S is now a percentage of EACH region's source width and height.
  Every region and axis uses its own sample-lattice ceiling, slightly below
  50%; a narrow region no longer limits larger ones. C still uses the whole
  source frame. S defaults to25%, with Cross/R50/Q25/C3/zoom1.00, cutoff1Hz,
  damping0.9 and bilinear output. Yellow bidirectional X/Y arrows replace the
  search rectangles. The origin marks zero displacement; diagonal searches
  remain possible. A focused search preview shows one region's actual pixels.
  Period is displayed in seconds: below1s uses one decimal, at/above1s an
  integer. Positive periods below0.1s show <0.1s. The exact input stays Hz.
  This release intentionally discards pre2.8 processing settings and previous
  personal-default backups. It starts from the new general defaults; language
  and icon preferences remain separate. Newly saved My default and local undo
  use only schema9 / format2. No legacy geometry or unit-adoption control remains.
  See validation/region-search-browser-2.8.0.json. Earlier version descriptions
  below are historical and do not describe the current compatibility policy.

2.7.2 logarithmic cutoff and focused common controls
  Cutoff slider travel is logarithmic: equal distances represent equal ratios
  of frequency. Its existing 0.0001..5 Hz span is retained; precise input still
  accepts 0.0001..120 Hz. The numeric field and saved profile remain in Hz.
  A period readout shows 1000 / Hz in milliseconds (1 Hz = 1000 ms; 2 Hz =
  500 ms). This reference period is not processing latency or a filter time
  constant. Numeric precision remains four decimal places. Slider keys move
  1% of the logarithmic span; Shift/Page keys move ten steps. Text-field arrow
  keys retain the existing precise Hz nudges. Home/End select positive bounds.
  Cutoff and compensation C% are in the common controls with detection mode.
  Central region R, sampling Q and zoom are under Advanced. Moving/collapsing
  fields never changes their settings or the chosen processing workload.
  Apply reveals Advanced if a hidden field has an invalid draft. Existing
  custom profiles, comparison, undo and My default remain intact.
  Verification: validation/log-cutoff-browser-2.7.2.json.

2.7.1 simpler cutoff control
  Cutoff now appears in the common controls as one numeric input and slider.
  Heavy / Medium / Light are text guides, not extra preset buttons. Lower values
  follow camera motion more slowly; Medium marks the default 1 Hz position.
  The slider keeps its 0.0001..5 Hz range and precise entry keeps 0.0001..120 Hz.
  Editing cutoff changes no C, geometry, sampling, zoom or other parameter.
  Actual stabilization also depends on C and the footage; lower cutoff is not
  a guarantee of less measured shake in every clip. Original comparison, local
  undo and My default remain available. Existing 2.7.0 profiles keep both their
  saved cutoff and C; no automatic remapping or stored-profile conversion occurs.
  See validation/cutoff-browser-2.7.1.json. The 2.7.0 preset descriptions below
  are historical; their coupled cutoff/C buttons were removed in 2.7.1.

2.7.0 strength, comparison and recoverable profiles
  Light / Medium / Heavy prepare a draft; Apply to this video commits it.
  They change only cutoff and C: Light 1.5 Hz / 2.5%, Medium 1 Hz / 3%,
  Heavy 0.6 Hz / 5%. Mode, R, Q, S, zoom, damping, trust and interpolation
  remain yours. These are tested starting points, not scene recognition or a
  guarantee that heavier always looks better. Stronger smoothing follows pans
  more slowly and can expose more edges. General defaults remain Medium,
  Cross/R50/Q25/S6.25/C3, zoom1.00 and bilinear output.
  Compare original switches only the displayed picture; analysis continues.
  Return shows the latest stabilized frame. Comparison does not save settings,
  change the video/audio, or add undo history. Apply, a new video or an error
  ends comparison. Seeking and a quality change within the same video keep it.
  Cancel edits discards a draft. Undo last apply restores a complete previous
  processing profile, up to five committed changes in this viewing. General
  defaults and Use my default apply locally and can also be undone.
  This video means this viewing: navigating to another video or refreshing
  loads My default and clears local undo history. Other currently open videos
  keep their active settings. Save as my default explicitly saves the currently
  applied profile for later videos; apply any draft first. Restore previous
  default recovers the preceding saved profile without changing this video.
  Upgrading reads the existing custom profile without overwriting its original
  storage record. Old independent axes stay active until Use R / S / C is
  explicitly previewed and applied. Language and icon preferences save
  separately. Save failures preserve current playback and can be retried;
  unreadable saved defaults cannot be overwritten before a successful read.
  Verification: validation/profiles-browser-2.7.0.json. Earlier sections below
  document previous features; the storage scope described here takes priority.

2.6.0 supported inputs and movable player icon
  Numeric text inputs accept four decimal places independently of slider steps.
  Sliders retain common working ranges; focusing one never replaces an exact
  value outside its travel. Defaults remain Cross/R50/Q25/S6.25/C3/zoom1.00,
  cutoff1/damping0.9, with bilinear output. Existing profiles are preserved.
  R: 0..100%; R=0 works for X/adaptive corners, not an empty Cross/single layout.
  Q: 0.0001..100%; each actual sample axis still has at least 8 samples. Native
  axis/memory capacity is checked; slow processing does not reduce Q.
  S: requested 0..50%; actual shared search stays within each sample lattice.
  C: requested 0..204800%; actual shared C cannot exceed 65536 source pixels
  on either axis. Source changes retain the request and show its effective cap.
  Zoom: 0.0001..32768 (this implementation's tested input limits, not universal
  browser limits). Below 1.00, a black matte covers the unscaled original video.
  Cutoff: 0.0001..120 Hz; effective cutoff is at most half the processing frame
  rate. Damping: zero through the largest finite single-precision float.
  Trust: 0.1..100; large-motion penalty: 0..10. Subpixel remains only 0 or 1.
  Native normal-profile comparisons are retained. Stiff nonlinear correction
  uses an implicit solve instead of overflowing and resetting motion history.
  The player icon avoids the actual control strip and can be dragged. Arrow
  keys move it (Shift uses larger steps); Home or Reset icon position restores
  automatic placement. Show player icon can hide it without disabling output.
  Reopen settings from the extension toolbar popup to show it again. Icon
  preferences save independently, survive processing Reset defaults, and never
  reset motion analysis. See validation/limits-icon-browser-2.6.0.json.

2.5.2 compensation edge band
  C now uses a translucent purple edge band. Left/right thickness is source
  width times C%; top/bottom thickness is source height times C%. The inner
  rectangle subtracts both edges. Larger C makes the band thicker. C=0 has no
  band; overlapping opposite bands cover the frame without reducing C.
  C remains independent of search S. The band is a soft reference, not a crop
  or a guarantee against exposed edges; actual compensation can exceed C.
  The actual motion arrow and white visible-crop outline remain separate.
  Draft/Apply, five-second expiry and unequal legacy-axis settings are retained.
  Validation: validation/compensation-browser-2.5.2.json.

2.5.1 sliders and matching colors
  Every numeric field pairs a native slider with its precise text input.
  Drag/click for convenient steps; the text field retains finer accepted values.
  Arrow keys adjust, Shift or PageUp/PageDown use larger steps, Home/End select
  the bounds. Slider keys stay inside the settings panel, not YouTube shortcuts.
  Both controls update the same draft and five-second preview. Focusing a field
  shows its relevant region without changing or saving it; Apply still commits.
  R uses blue outlines, Q teal sample labels, S yellow search boxes, C purple
  compensation, and Zoom white crop outlines. Labels, field accents, slider,
  legend and focused preview title share one palette. Other numeric parameters
  use a neutral color because they do not define a separate spatial box.
  Candidate/analyzed/accepted status uses fill and small gray/blue/green dots;
  an accepted region does not recolor the R outline. Defaults and core unchanged.
  Validation: validation/sliders-browser-2.5.1.json.

2.5.0 shared ratios and five-second region preview
  R is the central width/height percentage; S is one source-relative search
  percentage for both axes; C is one source-relative soft compensation limit.
  The old layout selector, custom width/height, auto/manual search selector and
  separate X/Y search/limit fields are removed from the form. New defaults are
  Cross five, R50, Q25, S6.25, C3 and zoom1.00. S/C are engineering starting values.
  S is capped to a common range supported by all candidate sample grids; the
  requested value is retained and the effective ceiling is displayed. S measures
  motion between processed frames, while C limits accumulated/smoothed output.
  Changing a valid parameter shows a preview for five seconds from the last
  edit. Apply or Show regions displays it again. Dashed geometry is a draft;
  applied regions use actual selections/inliers, with no guessed adaptive votes.
  Gray marks candidates, blue analyzed/planned regions, green accepted regions;
  yellow is the search displacement, purple soft compensation, white visible
  zoom crop. Q shows sample dimensions within unchanged analysis regions.
  Search boxes do not imply reading extra image area; C is not a hard crop.
  The overlay uses the same output coordinates and actual translation, handles
  letterboxing/zoom/mirroring and does not intercept input or change video pixels.
  Seeking, source changes, disable and controller destruction clear it.
  Existing profiles remain active under compatibility handling. Use R / S / C
  prepares a draft and Apply adopts it. Equal old percentages are retained;
  non-equivalent settings use displayed starting values. Old axis data remains
  stored but inactive after adoption. Other user preferences are preserved.
  Scoped evidence: validation/overlay-browser-2.5.0.json.

2.4.1 lifecycle repair (retained)
  Disabling or reloading the Chrome extension retires the old content script:
  remove its controls/output, stop callbacks/listeners and abort pending loading.
  The next player tick or page/video event detects invalidation; background-tab
  timer throttling can delay the tick. Re-enable, then refresh existing YouTube
  pages to start a fresh context. This release cannot retrofit cleanup into an
  already-running 2.4.0 script; refresh once after updating.
  Player icons now use the same original SVG inline, without an external URL.
  WASM loads once as bytes and compiles through the supported instantiateWasm
  hook. Actual fetch/compile failures remain visible and retryable. The native
  core, detection settings and saved profile are unchanged.
  The player's Enable stabilization checkbox still keeps its dimmed entry so
  stabilization can be turned back on; Chrome extension disable removes it.
  See validation/lifetime-2.4.1.json for scoped tests and remaining live checks.

Real-time, translation-only video stabilization inside the YouTube player.
The DePan / FFTW WebAssembly core runs on your device. YouTube still controls
audio, seeking, speed and fullscreen. No preliminary download or conversion.

Install / share
  The Video-Stabilizer-2.9.5.zip archive contains the extension itself.
  Extract it into one folder. In desktop Chrome, open Extensions > Manage
  extensions, enable Developer mode, choose Load unpacked, and select that
  folder. Keep the folder, including the .wasm file and _locales directory.
  This is an unpacked extension package, not a Chrome Web Store listing.
  When updating an existing unpacked copy, replace its files, reload the
  extension, then refresh already-open YouTube pages.

Use
  Open a regular www.youtube.com/watch video and select the camera icon at
  the lower right of the player. Enable or disable stabilization in its panel.
  Edit the fields and choose Apply or press Enter; later videos use these values.
  Save as my default is enabled after Apply and saves the confirmed settings.
  Closing the panel discards unapplied edits. Restore my default loads the
  one saved profile; it is unavailable until a valid profile has been saved.
  System defaults fills the form with central only, R85/Q30/regional S30/C15,
  cutoff0.5Hz/damping0.3 and 1.00x, keeping language and icon preferences.
  Both preset buttons require Apply; closing cancels their unapplied values.
  The current schema9/format2 personal profile remains available; old backups are ignored.
  Processing profiles older than2.8 are not loaded.
  New videos, tabs and reloads use the last Apply. My default is restored manually.
  Copying the extension to another computer does not copy browser settings.

Recognition
  A mint-green camera, central play symbol and paired stabilization arcs
  identify the extension in Chrome and inside the player. The same mark
  appears in the popup and website. Numeric settings and on/off controls
  remain in the player. The toolbar uses supplied PNGs at six sizes.
  The in-player entry is icon-only, with a localized accessible name.
  Its hover tooltip reports on/off/original state. Off or bypassed
  output dims the icon. Press Enter/Space to open it, or Escape to close.

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

Detection, ratios and resource choice
  The common panel contains four controls: Mode, central ratio R, sampling
  ratio Q and Zoom. Language, smoothing, shared search and soft limits are in
  Advanced. The original video controls and audio remain with YouTube.

  R defines the non-overlapping 3x3 partition. At R=50, source 1024x768 has a
  512x384 center, 256x192 corners, 512x192 top/bottom-middle cells and 256x384
  side-middle cells. R applies to both width and height, not directly to area.
  Cross five (new default) uses center plus top/bottom/left/right middle.
  X five uses center plus four corners. Central only and Adaptive remain.
  Center priority in Advanced doubles the center weight within agreeing cells.
  Adaptive still estimates up to five spatially distributed candidates.
  Zero-weight or smaller-than-32-source-pixel cells do not vote. R=100 becomes
  one full-frame region and loses independent foreground rejection.

  Q retains a percentage of EACH active region's source width and height.
  Q=50% means about 25% as many samples; Q=25% means about 6.25%. It is not a
  128/256px ceiling. Q=100% retains all source samples, including odd sizes.
  Integer rounding and an internal minimum of eight samples per axis apply.
  Start with 25%, then judge image quality and measured speed on your footage.
  Raising Q can improve detail at higher cost; it cannot restore detail that
  is absent from a low-quality source. No pixel counts need to be edited.
  The synthetic 360p-to-4K tests passed at Q25. A separate 216p case had higher
  error at Q25 and improved at Q50; the recommendation is a starting point,
  not a guarantee for every subject or source.

  The read-only workload preview updates before Apply. Its reference is
  1080p, R=50, Cross five and Q=25%. The FFT operation index is proportional
  to samples * (log2(width)+log2(height)), including forward/inverse transforms.
  Adaptive gives a range for different selected cells and rebuilding references.
  This is not CPU utilization or predicted fps. Decode, readback, rendering,
  FFT dimensions and hardware also affect timing. Working-data memory is an
  estimate, not the browser's total or its retained linear-memory allocation.
  Expand Playback performance for actual output fps and processing time.
  High load does not lower Q or turn stabilization off. Busy source frames are
  skipped, processing continues and the UI reports slower throughput. Expected
  processing gaps do not repeatedly reset the reference. At very low output
  rates, reduced temporal detail and additional display delay are unavoidable.
  Applying settings starts a fresh timing sample, so comparisons are meaningful.

  The native engine supports up to 8192 samples per axis with growing WASM
  memory up to 2 GiB. 360p through 4K at Q=100 are supported. These internal
  capacity limits are checked, not silently substituted with a lower Q.
  Actual allocation, restricted-frame or canvas failures restore original
  playback; reduce Q or correct the source and Apply to retry.

  Existing profiles retain their geometry, axis limits and sampling until
  Use R / S / C is selected and applied. No source resolution is guessed for
  old pixel settings. The preview makes non-equivalent changes reviewable.
  Older builds cannot interpret the unified model; use their own defaults or
  a compatible settings backup when downgrading.

Default parameters
  Mode             Central region only; center priority off.
  Central ratio R  85% of source width and height.
  Sampling ratio Q 30% of each region's source width and height.
  Search range S   30% of each region's source width/height, each axis capped independently.
  Zoom             1.00 (no enlargement; moving borders may expose black).
  cutoff/damping   0.5 Hz / 0.3; cutoff is common, damping is in Advanced.
  Limit C          15% of source width/height, native soft limits.
  trust/stab       4 / 1; joint confidence is a heuristic, not a probability.
  subpixel         1 (bilinear). Nearest-neighbor remains an advanced option.
  R replaces custom window width/height; S/C each use a single percentage.
  Pixel dimensions are diagnostic output or legacy data, not ordinary input.

Compatibility and limits
  Historical 2.3 results are in validation/ratio-browser-2.3.0.json. The final
  default R=50 synthetic 1080p/30 pixel test left about 28.7% of the original
  velocity at 30 fps, with 0/313 decoder drops in that interval. Source-detail
  single processing also matches the former path on 360 reference frames.
  The R=100 moving-foreground negative control remains in the report: one
  full-frame region cannot provide independent spatial agreement.
  Earlier 2.2 tests and earlier failed attempts are recorded in
  validation/regions-browser-2.2.0.json. The final default synthetic 1080p/30
  pixel test left about 32.6% of the original velocity, at 30.1 fps and 0/313
  decoder drops. An independent 8-second cadence interval measured 30 fps
  and 0/240 drops. These local synthetic results do not guarantee YouTube,
  other devices or continuous 4K performance.
  Desktop Chrome 120+ is required. Tested on Chrome 156 / Windows. Other
  Chromium browsers are not separately qualified. Normal 24-30 fps playback
  at 1x is the main validated use case. Higher speeds, 48/60 fps and 4K depend
  on the device and stream; reducing the analysis window is not guaranteed
  to improve cadence. The earlier 1080p/24 at 2x test did not reach all 48
  required output frames per second. Those are historical measurements.
  The earlier synthetic 1080p/30 comparison produced 29.2 fps in 2.1 and
  29.4 fps in 2.0, with dropped frames in both versions and the original
  player. The strict cadence checks did not pass. See
  validation/public-validation.json in the source package for measured
  results and their scope; these are not guarantees for every device.
  The 2.1.3 defaults, save/reset, foreground media and multilingual checks
  are recorded in validation/defaults-browser-2.1.3.json. It retains the
  failed direct-tab attempt as well as the successful foreground rerun.
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
  Public profile/link checks do not verify account
  eligibility, completion of a payment or withdrawal to a bank account.

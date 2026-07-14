# Application Submission

Walkie Talkie for Flipper Zero: a receive-only FRS channel activity and RSSI scanner. Tunes the built-in CC1101 to the 22 standard FRS channels (462/467 MHz) with auto-squelch, live RSSI meter, and an auto-pausing channel scanner. Receive-only; it does not transmit. See `docs/changelog.md` in the source repo for what changed in this version.

# Extra Requirements

- None. Uses the Flipper Zero's built-in CC1101 radio; no external hardware required.

# Author Checklist (Fill this out)

- [x] I've read the [contribution guidelines](../blob/HEAD/documentation/Contributing.md) and my PR follows them
- [x] I own the code I'm submitting or have code owner's permission to submit it
- [x] I have performed a self-review of my own code
- [x] I have commented my code, particularly in hard-to-understand areas
- [x] I [have validated](../blob/HEAD/documentation/Contributing.md#validating-manifest) the manifest file(s) with `python3 tools/bundle.py --nolint applications/CATEGORY/APPID/manifest.yml bundle.zip`

# AI usage disclosure (Fill this out):

- [x] Partially AI assisted (clarify below which code was AI assisted and briefly explain what it does).
- [ ] Fully AI generated (explain what all the generated code does in moderate detail).

- AI assistance was used for portions of the app code and for preparing/validating this catalog manifest and submission. The app tunes the built-in CC1101 to FRS channels and reports channel activity/RSSI.

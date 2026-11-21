CW DECODER (DeepCW + HamNoise) for Mac (Apple Silicon)
===================================================

Install
1. Drag CW DECODER.app into the Applications folder.
2. The app is not signed with an Apple certificate (local "ad hoc"
   signature only), so macOS blocks it on first launch. Unblock it either:
   a) in Terminal:  xattr -dr com.apple.quarantine "/Applications/CW DECODER.app"
   b) or try to open it, then System Settings > Privacy & Security >
      "Open Anyway".
3. On first launch allow microphone access (needed to read the USB audio
   input).

Use
- Press Start, then open Settings and pick your radio's USB audio
  interface under "Input".
- "Monitor output": where to hear the audio (headphones/speakers).
- Noise reduction (HamNoise):
    Off                no noise reduction
    Monitor only       cleans only the audio you hear (default)
    Monitor + decoder  also feeds the cleaned audio to waterfall and decoder
- Language: Italiano or English, in Settings > Appearance or in the
  Language menu. On first launch it follows the system language.
- A- / A+ change the text size, "Copy text" puts it on the clipboard,
  "Clear" empties it. Callsigns are highlighted in amber.
- The Settings button hides the side panel.
- Click the waterfall to move the decoding passband, scroll to fine-tune.
- Pileup mode decodes several signals at once. Engine: WASM or WebGPU.

Everything runs locally, with no network.

Credits
DeepCW   https://github.com/e04/web-deep-cw-decoder  (MIT, (c) 2026 e04)
HamNoise https://github.com/e04/HamNoise             (MIT, (c) 2026 e04)

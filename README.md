# dictate

A free Windows dictation tool. Hold a key, talk, let go. The words appear where your cursor is, in any app, in English or Polish.

**[Download dictate for Windows](https://github.com/michalszyszka2-cmyk/dictate-download/releases/latest/download/dictate-setup.exe)** (about 37 MB, Windows 10 or 11, 64-bit)

## Install

1. Run `dictate-setup.exe`. It installs for your user only, no admin rights needed.
2. Windows may say "Windows protected your PC" because the app is not code-signed. Click **More info**, then **Run anyway**.
3. On first start dictate downloads the speech model (about 720 MB). The tray icon shows progress. Dictation turns on when it finishes.

## Use

- Hold **Right Shift**, speak, let go. The text is pasted where your cursor is.
- **Esc** while holding cancels.
- Click the green tray icon to turn dictation off and on.
- Right-click the tray icon, then **Settings**, to change the keys and the clean-up step.

Speech is recognised on your own PC, so nothing leaves it by default.

## Clean-up (optional)

Clean-up fixes grammar, punctuation and filler words. It is off until you pick who does it in **Settings**:

- an **OpenRouter** key (has free models),
- a **Claude** API key or an **OpenAI** API key (pay as you go, a tiny fraction of a penny a clip),
- or your own **Claude** or **ChatGPT** plan, through Claude Code or Codex installed on your PC. No key needed, but each clip takes several seconds.

When clean-up is on, the text of each clip (not the audio) goes to the service you picked.

## Ask box (optional)

Hold **Right Shift + Right Ctrl** and ask a question. It goes to Claude Code on your PC and the reply shows in a small box. Needs [Claude Code](https://claude.com/claude-code) installed and signed in.

## Update or remove

Run a newer `dictate-setup.exe` over the old one; your settings are kept. To remove, use Windows Settings → Apps → dictate.

## Credits

Speech recognition: [NVIDIA Parakeet TDT 0.6B v3](https://huggingface.co/nvidia/parakeet-tdt-0.6b-v3), licensed [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/), run through [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) in a converted int8 form.

Free to download and use. Made by Michal Szyszka.

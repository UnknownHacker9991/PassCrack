# PassCrack — Password Strength Analyzer

A web-based password strength analyzer that simulates real attack techniques to show how fast your password could be cracked. All analysis runs locally in your browser — no data is ever transmitted.

## Features

- Real-time strength scoring as you type (0–100 scale).
- Estimated crack times across 4 attack scenarios (online, offline slow/fast hash, GPU cluster).
- Pattern detection: common passwords, dictionary words, l33t speak, keyboard walks, sequences, dates, repeated characters.
- Entropy calculation based on actual character pool size.
- Visual breakdown: length, charset diversity, entropy bits, pattern count.
- Actionable vulnerability feedback with severity ratings.
- Dark themed, responsive UI — works on mobile.

## How It Works

The analyzer checks your password against multiple real-world cracking techniques:

| Technique | What it does |
|---|---|
| **Common password check** | Tests against the top 200 most-used passwords |
| **L33t speak decode** | Converts substitutions (@ → a, 3 → e) and re-checks |
| **Dictionary attack** | Scans for embedded common English words |
| **Pattern detection** | Finds keyboard walks (qwerty), sequences (abc, 123), repeats (aaa) |
| **Brute force estimate** | Calculates time based on password length × character pool size |

## Usage

Just open `index.html` in any browser. No server, no dependencies, no install.

Or host it on GitHub Pages:
1. Push to a repo
2. Go to Settings → Pages → Source: main branch
3. Your analyzer is live at `https://yourusername.github.io/passcrack/`

## Privacy

Zero data leaves your browser. The entire analysis runs in client-side JavaScript. No API calls, no tracking, no cookies.

## Built With

- HTML / CSS / JavaScript (single file, no dependencies)
- JetBrains Mono + Outfit fonts (Google Fonts CDN)

## License

MIT

## Co-Authored-By: Claude <81847+claude@users.noreply.github.com>

# Radix Calculator 🧮

A Casio-style scientific calculator that runs in your browser, installs on Android and iPhone, and works fully offline.

🚀 **Try it now:** [radix-calculator.vercel.app](https://radix-calculator.vercel.app/)

I've deployed Radix Calculator so you can open it directly in your browser and try its features. Install it on your phone for a calculator experience that works even without an internet connection.

No account. No tracking. No network calls after the first load.

## Features

### Calculator
- Scientific keypad with trigonometry, hyperbolic functions, logarithms, powers, roots, factorial, nPr, nCr, Pol/Rec, GCD, LCM, Int, Intg, Ran# and RanInt.
- Fractions with S⇔D conversion, exact results as π multiples and surds.
- Degree, radian and gradian angles, with DMS entry and display (° ′ ″).
- Display formats: Norm 1, Norm 2, Fix, Sci and Eng.
- Memory (M+, M−, MR), Ans and variables A–F, X, Y and M.
- 40 physical constants.
- Numerical integration, differentiation and summation.
- Calculation history.

### Modes

| Mode | What it does |
|---|---|
| Complex | a + bi and r ∠ θ arithmetic, powers and roots |
| Base-N | BIN, OCT, DEC, HEX conversion and bitwise operations |
| Stats | Mean, spread, regression and best-fit line |
| Distribution | Normal, binomial and Poisson distributions |
| Solve | Equations up to 4th degree, systems of equations and f(X) = 0 |
| Inequality | Polynomial inequalities |
| Matrix | Determinants, inverses and multiplication |
| Vector | 2D and 3D operations |
| Calculus | Integration, differentiation and summation |
| Ratio | A : B = X : D and A : B = C : X |
| Spreadsheet | 45 rows × 5 columns, cell references and built-in functions |
| CALC | Recalculate expressions using new variable values |
| Verify | Check whether a mathematical statement is true or false |
| Table | Calculate values of f(x) over a range |
| Convert | Length, mass, temperature and more |
| QR Code | Generate QR codes from results or text directly on your device |

## Quick start

The app uses plain static files and requires no build step. The deployed version is available here:

**🌐 [Open Radix Calculator](https://radix-calculator.vercel.app/)**

Open the link and start calculating. To install it on your phone and use it offline, follow the steps below.

### Install on Android

1. Open the website in Chrome.
2. Tap the ☰ DEG menu.
3. Select **Install app** and confirm.

You can also use Chrome's menu to install the app.

### Install on iPhone and iPad

1. Open the website in Safari.
2. Tap **Share**.
3. Select **Add to Home Screen**.
4. Tap **Add**.

The calculator will open from your home screen like a regular app.

## Offline use

1. Open the hosted app once while connected to the internet.
2. Open the ☰ DEG menu.
3. Wait until the menu displays **Ready offline**.

After the files have been cached, the calculator can run without an internet connection.

All calculation modes, history, spreadsheet features, constants and QR code generation are designed to work offline.

## Privacy

- Calculations and QR codes are generated on your device.
- No account is required.
- No analytics or advertisements.
- Spreadsheet content and settings are stored in your browser's local storage.
- The app is designed to make no network requests after the initial files have been loaded, except when checking for updates.

## Project files

| File | Purpose |
|---|---|
| `index.html` | Calculator interface, styling and JavaScript |
| `manifest.webmanifest` | App name, colours and installation settings |
| `sw.js` | Service worker for offline caching |
| `icon-192.png` | App icon |
| `icon-512.png` | High-resolution app icon |
| `apple-touch-icon.png` | iPhone home screen icon |
| `_headers` | Hosting configuration for service worker caching |
| `fonts/` | Bundled DM Mono and Barlow Semi Condensed fonts |
| `LICENSE` | MIT License |
| `THIRD-PARTY-NOTICES.txt` | Third-party licence notices |

## Updating

The hosted version can be updated by deploying the new files to the same hosting project.

When online, open the app and use **☰ DEG → Check for update** to fetch the latest version.

## Troubleshooting

| Problem | Fix |
|---|---|
| Install option is missing on Android | Use Chrome and open the HTTPS website directly. |
| Offline status never appears | Open the hosted website directly in a supported browser, not inside a preview frame. |
| No installation prompt on iPhone | Use Safari and select Share → Add to Home Screen. |
| Page not found | Ensure `index.html` is at the root of the deployed directory. |
| Old version still appears | Check for updates, then close and reopen the app. |
| QR code will not scan | Increase screen brightness, hold the camera steady and shorten long text. |

## License

Radix Calculator is released under the MIT License. You may use, copy, modify and distribute it, including commercially, provided the copyright and licence notices are retained.

### Third-party software

- DM Mono and Barlow Semi Condensed fonts — SIL Open Font License 1.1.
- qrcode-generator 1.4.4 by Kazuhiko Arase — MIT License.

Full notices are available in `THIRD-PARTY-NOTICES.txt`.

*Note: Numerical calculations use standard double-precision arithmetic, so very large or very small values may have minor rounding differences compared with dedicated hardware calculators.*

---

**Built for everyday calculations, advanced mathematics and offline convenience.**

🚀 **Try it today: [radix-calculator.vercel.app](https://radix-calculator.vercel.app/)**

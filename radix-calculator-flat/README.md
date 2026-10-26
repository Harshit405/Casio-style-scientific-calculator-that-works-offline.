# Radix Calculator

A Casio-style scientific calculator that runs in the browser, installs on Android and iPhone, and works fully offline. No account, no tracking, no network calls after the first load.

## Contents

- [Features](#features)
- [Quick start](#quick-start)
- [Install on a phone](#install-on-a-phone)
- [Offline use](#offline-use)
- [Using the menu](#using-the-menu)
- [Updating](#updating)
- [Privacy](#privacy)
- [Project files](#project-files)
- [Troubleshooting](#troubleshooting)
- [License](#license)
- [Third-party software and licences](#third-party-software-and-licences)

## Features

**Calculator**
- Scientific keypad with trig, hyperbolic, log, powers, roots, factorial, nPr, nCr, Pol/Rec, GCD, LCM, Int, Intg, Ran#, RanInt
- Fractions with S⇔D conversion, exact results as π multiples and surds
- Degree, radian and gradian angles; DMS entry and display (° ′ ″)
- Display formats: Norm 1, Norm 2, Fix, Sci, Eng
- Memory (M+, M−, MR), Ans, variables A–F, X, Y, M
- 40 physical constants
- Numerical integration, derivative and summation (∫, d/dx, Σ)
- History

**Modes**

| Mode | What it does |
| --- | --- |
| Complex | a + bi and r ∠ θ arithmetic, powers, roots |
| Base-N | BIN, OCT, DEC, HEX conversion and AND, OR, XOR, NOT, shifts |
| Stats | Mean, spread, regression and best-fit line |
| Distribution | Normal, binomial and Poisson |
| Solve | Equations up to 4th degree, 2 and 3 unknown systems, f(X) = 0 |
| Inequality | Polynomial inequalities |
| Matrix | Determinant, inverse, multiply |
| Vector | 2D and 3D operations |
| Calculus | Integral, derivative, sum |
| Ratio | A : B = X : D and A : B = C : X |
| Spreadsheet | 45 rows by 5 columns, A1 references, Sum, Mean, Min, Max, Prod, Count, fill down |
| CALC | Re-run an expression with new variable values |
| Verify | Check whether a statement is true or false |
| Table | Values of f(x) over a range |
| Convert | Length, mass, temperature and more |
| QR Code | Turn a result or any text into a QR code, generated on the device |

## Quick start

The app is plain static files. It needs hosting once so a phone can install it.

1. Unzip this package.
2. Put the folder on any static host that serves HTTPS.
   - **Netlify Drop:** open <https://app.netlify.com/drop> and drag the unzipped folder onto the page.
   - **GitHub Pages:** upload every file to a repository, then enable Pages under Settings.
3. Open the web address on your phone.

Installing and offline use need an `https://` address (or `localhost`). Opening the files directly from storage will not register the offline cache.

## Install on a phone

**Android (Chrome)**
1. Open the app address.
2. Tap **☰ DEG**, then **Install app**, then confirm.
   You can also use Chrome's menu, then **Install app**.

**iPhone and iPad (Safari)**
1. Open the app address in Safari.
2. Tap **Share**, then **Add to Home Screen**, then **Add**.
   Apple does not let a web page open this screen itself, so on iPhone the menu shows these steps instead of a one-tap button.

After installing, the app opens full screen from its own icon.

## Offline use

1. Open the app once while online. The first load saves every file on the phone.
2. Tap **☰ DEG**. The line at the bottom of the menu reads **Ready offline** when saving is done.
3. From then on the app opens and works with no internet.

Everything works offline: all modes, history, the spreadsheet, constants and QR codes.

### Single-file version

`radix-calculator-offline.html` has the fonts and QR maker built in and needs no hosting.

- **Android:** copy it to the phone and open it in Chrome from the Files app.
- **Limits:** it cannot be installed to the home screen, and iPhone cannot open local HTML files. Use the hosted package on iPhone.

## Using the menu

Every setting lives behind the **☰ DEG** button.

- **Angle unit:** Degree, Radian, Gradian
- **Modes:** open any mode from the grid
- **Setup:** Fix, Sci, Eng and fraction display
- **Copy result:** copy the answer on screen
- **Install app:** add to the home screen
- **Check for update:** fetch the latest version (shown when the app is running from a host)

## Updating

1. Upload the new files to the same host, replacing the old ones.
2. On the phone, tap **☰ DEG**, then **Check for update**, or just open the app while online.

The cache name changes with every build, so old files are removed automatically and no manual clearing is needed.

## Privacy

- All calculations and QR codes are made on your device.
- Nothing is sent to any server. There are no analytics, ads or accounts.
- Spreadsheet content and settings are kept only in your browser's local storage.

## Project files

| File | Purpose |
| --- | --- |
| `index.html` | The whole calculator (HTML, CSS and JavaScript in one page) |
| `manifest.webmanifest` | App name, colours and icons for installing |
| `sw.js` | Service worker: versioned offline cache |
| `icon-192.png`, `icon-512.png` | App icons (the 512 icon also serves as the maskable icon) |
| `apple-touch-icon.png` | iPhone home screen icon |
| `LICENSE`, `THIRD-PARTY-NOTICES.txt` | Licence terms |
| `fonts/` | DM Mono and Barlow Semi Condensed, bundled so no font is fetched online |

## Troubleshooting

| Problem | Fix |
| --- | --- |
| No **Install app** button on Android | Use Chrome, open the hosted `https://` address, and make sure it is not a private window. If the app is already installed the button is hidden. |
| Menu never reaches **Ready offline** (it may say "Saving the app for offline use…" or "This browser cannot save apps for offline use") | The page is not on `https://`, is inside a preview frame, or the browser is unsupported. Open the hosted address directly in Chrome or Safari. |
| iPhone shows no install prompt | Expected. Use Safari, then Share, then Add to Home Screen. Other iPhone browsers may not offer it. |
| Old version still showing | Tap **☰ DEG**, then **Check for update**, then fully close and reopen the app. |
| Offline file will not open on iPhone | iPhone cannot open local HTML files. Use the hosted package. |
| QR code will not scan | Shorten the text, increase screen brightness, and hold the camera steady. Very long text makes dense codes. |

## License

Radix Calculator is released under the [MIT License](LICENSE). You may use, copy, modify and distribute it, including commercially, as long as the copyright and licence notice are kept.

## Third-party software and licences

- **DM Mono** and **Barlow Semi Condensed** fonts, SIL Open Font License 1.1 (texts in `fonts/`)
- **qrcode-generator** 1.4.4 by Kazuhiko Arase, MIT licence (embedded in `index.html`)

Full notices are in `THIRD-PARTY-NOTICES.txt`.

The numerical results are computed in standard double precision, so very large or very small values can show small rounding differences from a hardware calculator.

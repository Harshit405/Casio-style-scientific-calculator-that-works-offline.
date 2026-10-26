RADIX CALCULATOR - works offline, installs on Android and iPhone
=================================================================

TWO WAYS TO USE IT OFFLINE

A) Installable app (recommended): needs hosting once, then works offline forever
   1. Put this folder on any free web host (an https address):
      - Netlify Drop: open https://app.netlify.com/drop, unzip this file, drag the folder onto the page.
      - or GitHub Pages: upload every file to a repository, then Settings > Pages.
   2. Open the address on the phone while online. The first load saves everything on the phone.
      Tap the DEG button (top left): the menu shows "Ready offline" when it is done.
   3. Install it:
      Android, Chrome: DEG menu > Install app (one tap), or Chrome menu > Install app.
      iPhone and iPad, Safari: Share > Add to Home Screen > Add.
      (Apple does not let a page open that screen itself, so on iPhone the menu shows the steps.)
   After that the app opens full screen with no internet. To update, upload the new files and
   tap DEG > Check for update (or just open the app while online).

B) Single file, no hosting: radix-calculator-offline.html
   Everything is inside the one file (fonts and QR code maker included).
   On Android: copy it to the phone, open it with Chrome from the Files app. It works with no internet.
   It cannot be installed to the home screen and iPhone cannot open local HTML files, so use A on iPhone.

WHAT WORKS OFFLINE: every mode, history, the spreadsheet, constants, QR codes (made on the device).
Nothing is ever sent anywhere.

FILES
  index.html            the calculator
  manifest.webmanifest  app name, colours and icons
  sw.js                 offline cache (versioned)
  icon-192.png, icon-512.png, apple-touch-icon.png
  fonts/                DM Mono and Barlow Semi Condensed (SIL Open Font License)

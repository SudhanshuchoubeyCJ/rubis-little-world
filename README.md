# Rubi's Little World ♡

A mobile-first birthday storybook made for Rubi by Prince.

## Included
- Three-screen experience: gift/password entrance, memory storybook + candle game, final hug + letter.
- Four personal photos and one short video from the supplied ZIP.
- Personal media is AES-GCM encrypted in the `assets/` folder. The browser decrypts it only after the correct secret date is entered.
- Name: `Rubi`
- Password: the date you selected (spaces/capitalization do not matter).

## Publish it free with GitHub Pages
1. Extract this ZIP.
2. Open your GitHub repository (or create a new empty repository).
3. Upload **the contents** of this folder (`index.html`, `assets/`, and `README.md`) to the repository root.
4. Go to **Settings → Pages**.
5. Under Build and deployment, choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
6. Wait for GitHub Pages to publish and open the generated link on an Android phone.

Use HTTPS. Browser WebCrypto and encrypted media loading require a secure context; GitHub Pages provides HTTPS.

## Important privacy note
The personal photos and video are encrypted at rest in the published `assets/` directory. The entered password derives the decryption key in the browser; the password itself is not embedded in the site source. Anyone can still download the encrypted files and public website source. A date-based password is easy to guess, however, so this is privacy against casual viewing—not strong protection against a determined person trying guesses offline.

## Your voice note
No separate voice recording was included in the uploaded ZIP. If you want your voice in the last page, record a short `voice.mp3` and tell me; the current build does not pretend to contain one.

## Change the final letter
The current letter is included in `index.html` in the element with `id="letter"`. Replace that text with your final wording if you want to personalize it further.

## Files
- `index.html` — complete website
- `assets/*.enc` — encrypted personal photos/video

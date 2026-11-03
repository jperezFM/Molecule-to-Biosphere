# Molecule to Biosphere: installable app

This folder is the complete app. Put it on any website that uses **https**, and students can install it on Chromebooks, Windows and Mac laptops. Once it is installed and has opened once while online, it also works **offline**.

## What's in the folder

| File / folder | What it is |
|---|---|
| `index.html` | The app itself |
| `manifest.webmanifest` and the `.png` icons | Make it installable with its own name and icon |
| `sw.js` | Makes it work offline and delivers updates |
| `LICENSE-….txt` | Licenses for the 3D library and fonts (built into `index.html`) |

There are no subfolders: upload all of these files side by side.

## Step 1: Put it online (choose one)

**Option A: Your district's web server (recommended).** Send this folder to your tech department and ask them to host it at an https address, for example `https://www.yourdistrict.org/biology/`. They can also handle Step 2.

**Option B: GitHub Pages (free).**
1. Make a free account at github.com. Then create a new **public** repository, for example `molecule-to-biosphere`.
2. On the repository page, choose **Add file → Upload files**. Drag in **everything inside this folder** (not the folder itself), then click **Commit changes**.
3. Open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, select **main** and **/ (root)**, then click **Save**.
4. After a few minutes your app is at `https://YOUR-USERNAME.github.io/molecule-to-biosphere/`.

**Option C: Netlify Drop (free, quickest test).** Go to app.netlify.com/drop and drag this folder onto the page. It gives you an https address in seconds. Make a free account so the site doesn't expire.

> A free GitHub Pages or Netlify address is public: anyone with the link can open it. The app has no logins and collects nothing. Students' level choices and Journey progress are saved only on their own device.

## Step 2: Get it onto student devices

**Managed Chromebooks (best).** Your Google Workspace admin can install it for every student, with no action needed from students:
1. In the Google Admin console, go to **Devices → Chrome → Apps & extensions → Users & browsers**.
2. Select the students' organizational unit.
3. Choose **Add (+) → Add by URL** and paste the app's address.
4. Set the installation policy to **Force install + pin to ChromeOS taskbar**, then click **Save**.

Use the final address exactly as it appears in the browser, one that doesn't redirect anywhere else.

**Any Chromebook or laptop, by hand.** Open the address in Chrome or Edge. Then either click **Install app** at the top of the page, or click the install icon at the right end of the address bar. Molecule to Biosphere then opens in its own window and appears with the computer's other apps.

## Updating the app

Upload the new files over the old ones, replacing everything. The next time students open the app online, it downloads the update in the background and shows a **Reload** button.

## What works offline

Everything in the app works offline: the 3D zoom (including every place on the globe), the Journey, the labs, place pages and the built-in practice. Links to outside documents, such as the released Regents exams on nysedregents.org, need the internet.

## If the page stays on the loading screen

Check that **all** the files were uploaded side by side at the top level of the repository (not inside a folder), especially `index.html`, `sw.js` and `manifest.webmanifest`. After uploading new files, wait a few minutes for GitHub Pages to update, then reload with **Ctrl+Shift+R**.

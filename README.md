# CORVANE — Cinematic Archive

A responsive, single-file personal brand website for CORVANE.

## Included
- `index.html` — complete website, responsive styling, and simple interactions
- No build tools or dependencies required
- Placeholder visual backgrounds are made with CSS, so no image files are required yet
- Instagram links point to `https://www.instagram.com/corvane.wav/`

## Preview on iPhone
The easiest route is to publish using GitHub + Vercel (steps below). The site cannot become public merely by saving this file.

## Publish from iPhone using GitHub + Vercel
1. Sign in or create an account at https://github.com/
2. Create a new **public** repository named `corvane-cinematic-archive`.
3. In the repository, choose **Add file** → **Create new file**.
4. Name the file exactly `index.html`.
5. Open the downloaded `index.html` file from the Files app, copy all its contents, and paste into GitHub's editor.
6. Commit the new file to the repository.
7. Sign in at https://vercel.com/ and choose **Add New** → **Project**.
8. Import the `corvane-cinematic-archive` GitHub repository.
9. For a plain HTML site, no framework or build command is needed. If Vercel asks for a framework preset, choose **Other**; leave build command empty and use the repository root as the output/root directory.
10. Press **Deploy** and wait for Vercel to finish. Open the generated `*.vercel.app` URL to check the site.
11. Later edits to `index.html` committed to the connected GitHub repository normally trigger a new deployment automatically.

## Add your own photos later
The first version uses CSS gradients as artwork placeholders. To use your own photos:
1. In the GitHub repository, use **Add file** → **Upload files** and upload photos into an `images` folder (if the mobile UI makes folder creation awkward, upload a file named `images/your-photo.jpg` if supported, or create the folder on a computer).
2. Edit `index.html` and replace the relevant `<div class="art art-film"></div>` element with an image, for example:
   `<img class="art" src="images/japan-film.jpg" alt="Night street in Japan">`
3. Add `object-fit: cover; width: 100%; height: 100%;` to the image style if needed. The existing `.art` class is absolutely positioned; the image will fill the tile.
4. Commit the changes and wait for Vercel to redeploy.

## Custom domain later
1. Buy a domain from a domain registrar when ready.
2. In Vercel, open your project → **Settings** → **Domains** → add the domain.
3. Follow the exact DNS records Vercel shows for your domain registrar. Do not guess or copy generic DNS values; use the values displayed for your project.
4. Wait for DNS verification/SSL provisioning, then test the domain.

## Notes
- This file is a static site and does not collect personal information.
- The music area is a mood indicator only; it does not play audio.
- The website is not deployed by generating these files. You must complete the hosting steps above to get a public URL.

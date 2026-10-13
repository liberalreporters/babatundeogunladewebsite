# Image, News & Announcement Upload Guide
Repository: https://github.com/liberalreporters/babatundeogunladewebsite

## Exact image folders
- Official portrait: `assets/images/profile/` — suggested filename `babatunde-ogunlade-portrait.jpg`
- Biography/professional photo: `assets/images/profile/` — suggested filename `babatunde-ogunlade-professional-photo.jpg`
- Events/gallery: `assets/images/gallery/` — e.g. `eru-community-engagement-2026-10.jpg`
- News photos: `assets/images/news/` — e.g. `community-update-2026-10.jpg`
- Announcement graphics: `assets/images/announcements/` — e.g. `community-meeting-notice-2026-10.jpg`

## Upload from your phone
1. Open the repository link above and sign in to GitHub.
2. Open `assets` → `images` → the required folder.
3. Tap **Add file** → **Upload files**.
4. Select the image from your phone and wait for it to upload.
5. Enter a commit message such as `Add official profile portrait`.
6. Choose **Commit directly to the main branch** and tap **Commit changes**.

If a folder is missing, use **Add file** → **Create new file** and enter a path ending in `README.md`, for example `assets/images/news/README.md`. Commit it, then upload into that folder.

## Replacing a placeholder
This pack contains SVG placeholder images so you can identify each image slot. Uploading a JPG does not automatically replace an SVG or update the page. Upload the real image, then update the page or JSON `image` field to its exact path. Example:
`/assets/images/news/news-image-placeholder.svg` → `/assets/images/news/community-update-2026-10.jpg`

## Adding news
1. Open `news.json` in GitHub and tap Edit (pencil).
2. Replace the sample record or copy it for another story.
3. Use a unique lowercase ID with hyphens; set the date as `YYYY-MM-DD`.
4. Add headline, summary, image path, alt text, author and a source.
5. Keep `status` as `draft` until verified and approved; then set it to `published`.
6. Commit directly to `main`.
Use `content-templates/news-article-template.md` to draft the full story first.

## Adding announcements
1. Open `announcements.json` and tap Edit.
2. Replace or duplicate the sample record.
3. Fill in title, date, summary, full body, image path, alt text, confirmed start/end dates and authorised contact as relevant.
4. Keep `status` as `draft` until approved.
5. Commit directly to `main`.
Use `content-templates/announcement-template.md` to prepare the notice.

## Important limitation
JSON files are structured content templates. They will not automatically appear on the live site unless its HTML/JavaScript is configured to load and render them. The existing homepage has image-placeholder sections and `news.json` is a template. After uploading this pack, website code may still need to be connected to the portrait, gallery, news and announcements data. A GitHub commit alone does not guarantee that content appears live.

## Publishing checks
Verify names, roles, dates, venues, figures and quotations. Use accurate captions and meaningful alt text. Obtain image permission where needed. Never publish placeholder text as factual news.

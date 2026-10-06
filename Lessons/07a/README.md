# POLS 6394 — 07a: Publish Yourself

This project contains the materials for one class meeting. Today you build a PDF CV and a simple website. Both belong in your own GitHub account,
separate from your coursework repository. The website can stay private.

## Start here

1. Open `07a-workbook.qmd` in your coursework project. Keep it open for your notes.
2. Open the [07a slides](https://uh-pols6394-fall26.github.io/course-materials/Slides/07a-slides.html) in a browser. A local lesson copy also has `07a-slides.html`.
3. Follow the workbook to create the CV and website. Each gets its own folder
   and RStudio project, opened in a new session. Keep your coursework window open.

Both start from GitHub's **Use this template** button and open in RStudio with
**File → New Project → Version Control → Git**. The workbook explains each step.
In the clone dialog, set **Create project as subdirectory of** to `~` for both
projects. This is your home folder: `cv`, your site, and your coursework folder
should be siblings. Don't clone the CV or site inside the coursework folder.

For the website clone, set **Project directory name** to `YOURUSERNAME.github.io`
(public route) or `site` (private route). A beta project uses its actual repository
name. Keep **Create project as subdirectory of** set to `~`. The GitHub repository
name determines the published URL; the local folder name doesn't change it.

## Files and folders

- `07a-slides.qmd` and `07a-slides.html`: slide source and rendered slides
- `07a-workbook.qmd`: the student workbook and record of the class meeting

Rendered workbook output and RStudio session files are ignored because they can be regenerated.
The CV starter (`bshor/cv-starter`, a fork of Christopher Kenny's
`quarto-cv` template) and the website starter (`bshor/cv-minimal-site`) are
copied from GitHub during class.

## What to submit

- **By 7:00 PM Wednesday, October 7:** render, commit, and push your 07a workbook
  in the coursework repository. Record your progress and both repository URLs.
- **Thursday, October 15:** finish the CV and website, render both, and push
  their files to their own repositories. Give Amanda and me access.

A public website and a public CV link are optional.

## Copy your CV into the site, if you want the link

Choose one route; you don't need both.

**Files pane (no Terminal):**

1. In your CV window's **Files** pane, check the box beside the rendered PDF.
2. Choose **More → Copy To**. Browse to your website project and its `files`
   folder, then confirm the copy. Use **Copy**, not Move.
3. In the site's **Files** pane, open `files`. If the copied PDF has a different
   name, select it and click **Rename**; name it `cv.pdf`.
4. Render the website, check its CV link, then commit and push. Copy again
   whenever the CV changes. These steps also work in RStudio Server.

**Terminal alternative:**

In the site's RStudio Terminal, run `ls -l ..`. This lists the parent folder;
read the names at the end of the lines and find the folder from your CV step.
Its name may be `cv`, `fall26-6394`, or something else.

Run `ls -l "../CV_FOLDER"`, replacing `CV_FOLDER` with that name, to find the
rendered PDF. Then run `cp "../CV_FOLDER/cv.pdf" files/cv.pdf`. Replace the
source folder and PDF name as needed; keep `files/cv.pdf` as the destination
because that's what the website link uses. Quotes allow spaces in names.
Copy again after each CV update, then render the website.

If the CV folder isn't listed, check its recorded location rather than guessing.
Skip copying entirely if you want to keep your CV off the website.

## View your website on your computer

In your website's RStudio window:

1. In the **Build** pane, click **Render Website** to create or update `docs/`.
2. In **Files**, open `docs`.
3. Click `index.html` and choose **View in Web Browser**.

This opens the finished page locally. Clicking HTML on GitHub shows its source.
Keep the entire `docs/` folder together; it includes the page's pictures and styling.

## Keep the website private

1. Keep its GitHub repository **private**. Don't enable GitHub Pages.
2. Render, commit, and push the complete `docs/` folder along with your sources.
3. On GitHub, choose **Settings → Collaborators → Add people**. Invite `bshor`
   and `ataustin06`, then send us the repository URL.

A private repository controls access to its files. It does **not** make a
published GitHub Pages website private.

There is no hosted website URL for this route. Amanda and I view a downloaded
copy, as described in the next section.

## For Amanda and me: viewing a private site

1. Sign into your own GitHub account and accept the invitation.
2. Copy the repository's HTTPS URL from its green **Code** button.
3. In RStudio, choose **File → New Project → Version Control → Git**, paste the
   URL, check **Open in new session**, and create the project.
4. In **Files → docs**, click `index.html` → **View in Web Browser**.
   No render is needed to view the output already committed.
5. For updates, open this same project, click **Pull** in its Git pane, and
   refresh the browser page. Don't clone again. Stop if Pull reports a conflict.

## Publish the website publicly

1. Review the repository's contents, including `files/` and `docs/`. Unlinked
   files are public too. Include your CV only if you want it public.
   To leave it off, keep the navbar but change its CV item to `text: "Home"`
   and `href: index.qmd`. Don't copy the PDF. If you already
   copied it, delete both `files/cv.pdf` and `docs/files/cv.pdf` before rendering
   and pushing. Deleting a current file doesn't erase earlier public Git history.
2. If the repository is private, choose **Settings → General → Danger Zone →
   Change repository visibility** and make it public.
3. Render, commit the whole `docs/` folder, and push. Rendering only creates
   the files on your computer; it doesn't upload them. Open your repository
   on GitHub and confirm that `docs/index.html` is there.
4. Choose **Settings → Pages → Deploy from a branch**. Select `main`,
   folder `/docs`, and **Save**.
5. Open the repository's **Actions** tab and click the newest **pages build
   and deployment** run. Yellow means queued or running, a green check means
   success, and a red X means failure. Click a failed job to read its error.
   Check the run's time and commit so you aren't looking at an old failure.
   If no new run appears, confirm your push succeeded.
6. Once deployment succeeds, open the website link in **Settings → Pages**.

For your main professional site, name the repository exactly
`YOURUSERNAME.github.io` to get the shorter `https://YOURUSERNAME.github.io/`.
Other names produce `https://YOURUSERNAME.github.io/REPOSITORY/`. For example:

| Repository in the `borisshor` account | Website URL |
|---|---|
| `borisshor.github.io` | `https://borisshor.github.io/` |
| `beta-web-f26` | `https://borisshor.github.io/beta-web-f26/` |

Use the actual link in **Settings → Pages**, not a guessed address. Wait for
deployment to finish; a new site can briefly return 404.

If it still returns 404, check that GitHub has `docs/index.html`, then open
**Actions** and check the latest Pages deployment. If it failed because `docs/`
is missing, stage the complete folder in RStudio's Git pane, commit, and push.

After each website edit: **render → check in your browser → commit → push**.

## Try a different theme

Browse [Quarto's HTML themes](https://quarto.org/docs/output-formats/html-themes.html#overview)
and the [Bootswatch gallery](https://bootswatch.com/) for previews. In
`_quarto.yml`, change `theme: cosmo` to a theme such as `flatly`, `litera`,
or `darkly` (dark background). Render the website to see the change; commit
and push when you want to publish it.

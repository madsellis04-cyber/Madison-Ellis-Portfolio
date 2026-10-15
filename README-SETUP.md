# Madison Ellis portfolio update

This package adds a blog and photography gallery, and updates the portfolio title and welcome text. It does NOT include your existing `dolce.html`, `cmad.html`, `.wacz` archives or `replay` folder: keep those files in the repository.

## Install

1. Back up your current repository first (GitHub > Code > Download ZIP).
2. Upload the contents of this package to the ROOT of your existing GitHub repository, preserving folders and the leading dot in `.pages.yml`. Replace `index.html` and add the other files. **Do not delete any existing archive files.**
3. In GitHub > Settings > Pages, verify **Build and deployment** uses **Deploy from a branch**, `main`, `/ (root)` so GitHub Pages runs Jekyll. If your site currently uses a custom GitHub Actions workflow, do not switch blindly; adjust the workflow for Jekyll instead.
4. Wait for the GitHub Pages build to finish. Open `/blog.html` and `/photography.html` on your website.
5. Go to https://app.pagescms.org/, sign in with GitHub, and install/authorize the GitHub App for ONLY your `Madison-Ellis-Portfolio` repository. Choose your main branch. Pages CMS will read `.pages.yml`.
6. For a new blog post: Pages CMS > Blog Posts > New; enter title, date and body, then save. Your post will appear on the blog after GitHub Pages rebuilds. **Don't rename the generated post file**, since Jekyll expects filenames beginning `YYYY-MM-DD-`.
7. For photography: Pages CMS > Media > Photography — Upload Photos Here. Upload JPG/PNG/WebP images; they will appear in the photo-only gallery after GitHub Pages rebuilds. To remove an image, delete it in the media manager.

## Security

The Pages CMS login uses your GitHub account and repository write permissions. Keep 2FA on and authorize the GitHub App only for this repository. The blog and photo gallery are public, but visitors cannot publish unless they have repository write access. Anyone with your GitHub account access could publish.

## Notes

- Photo gallery displays images sorted by filename (reverse alphabetical), with no captions. For newest-first, name images like `2026-10-15-photo-name.jpg`.
- Posts use Jekyll; blog pages won't render correctly if opened as local files without a Jekyll build.
- If GitHub Pages is not building with Jekyll, `{{ ... }}` and `{% ... %}` may appear as text: verify Pages build configuration.
- The image editor is a third-party service; you must sign in and grant GitHub permissions yourself.
- You can continue to edit `index.html` in GitHub, but the blog and photos don't require HTML editing.

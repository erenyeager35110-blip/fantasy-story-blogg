DRAGONTALES BLOG + PAGES CMS SETUP

This is a one-time site setup. After the site works, use Pages CMS to create posts without editing code.

FILES
- .pages.yml: Pages CMS editor configuration
- src/content/posts/: stories (Markdown)
- Astro files: build the site pages
- public/images/: upload story images here via Pages CMS media manager

CLOUDFLARE PAGES SETTINGS
- Framework preset: Astro (or None if Astro isn't listed)
- Build command: npm run build
- Build output directory: dist
- Root directory: leave blank
- Production branch: main (if your GitHub default branch is main)

PAGES CMS
1. Go to https://pagescms.org/
2. Sign in with GitHub and authorize it.
3. Choose the fantasy-story-blog repository.
4. Pages CMS reads .pages.yml from the repository.
5. Open Posts / New entry, fill in title, description, date, category and story, then save/commit.
6. Cloudflare should rebuild automatically after each commit. New posts show after that deployment succeeds.

IMPORTANT
- Cloudflare dashboard itself does not have a blog-specific New Post button; Pages CMS is the publishing dashboard.
- First deployment must succeed before posts can be published to the live site.
- Adsterra is not added yet. Add its approved script to the site template only after the basic site deploys correctly.

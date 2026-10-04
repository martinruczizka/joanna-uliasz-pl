# Joanna Uliasz — website delivery

Dedicated public repository for the future Joanna Uliasz website.

Website target: `https://joanna-uliasz.pl/`.

## Release status

Infrastructure prepared; website content and release approval are pending. No live website has been deployed.

Only reviewed public website files belong in `site/`. Project documentation, CV evidence, private mail, account data and secrets belong in the separate private project repository.

## Deployment

GitHub Pages uses GitHub Actions. The workflow runs manually, on `main`, with explicit release confirmation. It requires `site/index.html`, `site/.nojekyll`, and `site/release-approved.json` containing `{"approved": true}`. These must be added after content approval, Polish language QA and device QA.

Only `site/` is uploaded. The workflow does not run on push. The custom domain and DNS will be connected at website release; mail DNS is managed separately.

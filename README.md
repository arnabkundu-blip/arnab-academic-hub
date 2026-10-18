# Arnab Kundu — Research Atlas

A static, responsive, single-file academic website and research dashboard.

## Run locally
Open `index.html` in a browser. For reliable API CORS handling, use a local server: `python3 -m http.server 8000` then visit http://localhost:8000.

## Data
The preview includes five publicly verifiable publications cited in INSPIRE author/coauthor records. The page requests live publication data from the INSPIRE-HEP public REST API on load or when Refresh is clicked. If API access/CORS/search fails, the preview remains. Live search uses author-name matching, not a verified INSPIRE author ID; results may be incomplete, especially for namesakes or pagination.

## Privacy
The research workspace saves notes and tasks in browser localStorage only. This is not a secure, authenticated private dashboard and should not hold confidential research.

## Deploy
Upload `index.html` to GitHub Pages, Netlify, Cloudflare Pages or any static web host. For production: add a server-side INSPIRE fetch with verified author recid, paginated fetching, scheduled daily sync (e.g. cron), a persistent database, user authentication for the workspace, and server-backed literature radar.

## Source links
- https://www.saha.ac.in/web/theory-personal-page?mid=730&tab=tab4
- https://saha.ac.in/web/thd-research
- https://inspirehep.net/authors?q=Arnab%20Kundu
- https://github.com/inspirehep/rest-api-doc

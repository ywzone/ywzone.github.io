# Yang Wang — personal website

Static site: Home, About & CV, Research & Publications, Blog. Plain HTML/CSS, no build step.

## File structure
```
site/
  index.html
  about.html
  research.html
  blog/
    index.html
    from-academia-to-industry.html   (starter post)
  assets/
    style.css
    images/    (profile photo, banner, research figures)
    docs/      (PhD thesis PDF)
```

## Editing content
Open any `.html` file in a text editor and edit the text directly — no build tools needed. To add a new blog post, copy `blog/from-academia-to-industry.html`, edit the title/date/body, and add a link to it in `blog/index.html`.

## Deploying to your Namecheap domain
Buying the domain on Namecheap doesn't include hosting — you need somewhere to serve these files. Two easy paths:

**Option A — Free static hosting (recommended, no server to manage)**
1. Push this `site/` folder to a GitHub repo, or drag-and-drop it into [Netlify Drop](https://app.netlify.com/drop) or [Vercel](https://vercel.com).
2. Once deployed, go to your host's domain settings and add your Namecheap domain as a custom domain.
3. In Namecheap → Domain List → Manage → Advanced DNS, add the DNS records your host gives you (usually an A record + CNAME, or "use these nameservers" for GitHub Pages).
4. Wait for DNS propagation (up to 24–48h, often much faster).

**Option B — Namecheap's own hosting**
If you bought a Namecheap hosting plan too (not just the domain), upload this `site/` folder's contents to the `public_html` directory via their File Manager or FTP (e.g. FileZilla), with `index.html` at the root.

## Suggested next steps
- Replace the "YW" circle on the home page with an actual photo (`<img>` inside `.hero-photo`).
- Add a downloadable CV PDF and link it from the About page.
- Write more blog posts as they come to you.

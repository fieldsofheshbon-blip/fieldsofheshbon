# Fields of Heshbon — website

Static site for fieldsofheshbon.com, hosted free on GitHub Pages.

Files: `index.html` (homepage), six town pages (`santa-fe/`, `eldorado/`, `tesuque/`, `nambe/`, `pojoaque/`, `arroyo-hondo/`), a `services/` folder with an all-services page and 14 service pages, an `about/` page for Bradley, a `guides/` folder with four articles, `og-image.png` (preview picture when the link is shared), `llms.txt` (a short site summary for AI tools), `styles.css` (shared look), `thanks.html` (shown after the form is sent), `logo.svg` (the badge, used in the header and browser tab), `logo-full.svg` (badge plus "FIELDSOFHESHBON Since 2021", for print, social media and cards), `sitemap.xml` and `robots.txt` (for Google), and `CNAME` (tells GitHub the domain).

Upload the town, services, guides and about folders too, keeping the folder structure. Dragging the whole folder's contents into GitHub's upload page does this.

## Put it online

1. **Make the repo.** Sign in at github.com, click **New repository**, name it `fieldsofheshbon`, set it to **Public**, and create it.
2. **Upload the files.** In the repo, click **Add file → Upload files**, drag in all the files from this folder, and click **Commit changes**.
3. **Turn on Pages.** Go to **Settings → Pages**. Under *Build and deployment*, choose **Deploy from a branch**, branch **main**, folder **/ (root)**, and save. The **Custom domain** box should fill in as `fieldsofheshbon.com`; if it doesn't, type it in and save.
4. **Point the domain at GitHub.** At the company where the domain was bought, open the DNS settings and add:
   - Four **A** records for `@`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - One **CNAME** record for `www` pointing to `YOUR-GITHUB-USERNAME.github.io`
   - Delete any old A or CNAME records for `@` or `www` (like a "parked" page).
5. **Turn on HTTPS.** DNS can take anywhere from a few minutes to a day to update. Once it does, go back to **Settings → Pages** and check **Enforce HTTPS**.

## Turn on the request form (one time)

The form sends to fieldsofheshbon@gmail.com through FormSubmit, a free service. Once the site is live, send one test request from the site. FormSubmit then emails that Gmail an **activation link**. Click it, and every request after that goes straight to the inbox. Check the spam folder if it doesn't arrive.

## Making changes

To edit text, open `index.html` on GitHub, click the pencil icon, make the change, and commit. The live site updates within a minute or two.

## Get found on Google

After the site is live, add it to Google Search Console (search.google.com/search-console), verify the domain, and submit `https://fieldsofheshbon.com/sitemap.xml`. Also set up a free Google Business Profile for Fields of Heshbon that lists the same six towns and links to the site.

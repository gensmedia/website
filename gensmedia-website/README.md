# gensmedia.com

The Gens Media website. One static page (`index.html`) with no build step, hosted on Vercel. The 3D lens in the hero is built with three.js 0.160, loaded from jsDelivr.

## What's here

| File | Purpose |
| --- | --- |
| `index.html` | The whole site: markup, styles, the 3D lens and scroll animation |
| `favicon.svg`, `apple-touch-icon.png` | Browser and home screen icons |
| `logo.svg`, `logo-512.png` | The Gens Media logo as a vector and a square icon |
| `og.png` | Image shown when the link is shared on social or in messages |
| `robots.txt`, `sitemap.xml` | Search engine discovery |
| `fonts/` | Self-hosted Geist and Geist Mono (SIL Open Font License), cached long term |
| `vercel.json` | Clean URLs, redirects from the old Wix paths, security and cache headers |

## Editing

Open `index.html` and change the text directly. Videos live in the `films` list near the top of the script at the bottom of the file. Each entry is a YouTube video ID, a title, a caption and a fallback color. Push to `main` and Vercel redeploys within a minute.

## The inquiry form

The form sends to hello@gensmedia.com through FormSubmit, a free form relay that needs no account. The first time someone submits, FormSubmit emails hello@gensmedia.com a one-time activation link. Click it, and every inquiry after that arrives as an email.

## Going live

1. Push these files to the `gensmedia/website` repository on GitHub.
2. In Vercel, choose **Add New > Project**, import `gensmedia/website`, and deploy. No settings need changing.
3. In the Vercel project, open **Settings > Domains** and add `gensmedia.com` and `www.gensmedia.com`.
4. Point the domain at Vercel where it is registered. If you bought it through Wix, change the DNS records in Wix to the ones Vercel shows you, or transfer the domain out of Wix first.
5. Once the new site loads on gensmedia.com, cancel the Wix plan. Download the hero video from the old site first, since it is not stored anywhere else.

## Search

After launch, add the site in Google Search Console and submit `https://gensmedia.com/sitemap.xml`.

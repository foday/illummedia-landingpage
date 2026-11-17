# Illummedia — free Astro landing page

Branding update: the wordmark uses a plain capital “I” (no lightbulb mark). The site uses “Collaborate” and “strategic alliances”; it does not use the unreleased product/domain name you asked to reserve.

This is a starter static landing page for Illummedia, built with Astro and designed for free static hosting on Cloudflare Pages.

## Before publishing

1. Open `src/pages/index.astro`.
2. Replace `hello@YOURDOMAIN.com` in the mailto link with an email address you control. If you do not have a domain email yet, use a contact email you can receive.
3. Update any wording, links, or claims so they accurately reflect what is currently available. This page is an early-access/coming-soon introduction, not a claim that all platform features are live.

## Cloudflare Pages build settings

- Framework preset: Astro
- Build command: `npm run build`
- Build output directory: `dist`
- Production branch: `main`

## Deploy without a terminal

1. Create a GitHub account and a new repository named `illummedia-website`.
2. Extract this ZIP on your computer.
3. In the GitHub repository, choose **Add file → Upload files** and upload the contents of this folder (not the enclosing folder itself).
4. Commit the files to the `main` branch.
5. In Cloudflare, open **Workers & Pages → Create application → Pages → Connect to Git**.
6. Connect GitHub and select `illummedia-website`.
7. Use the build settings above and deploy.
8. Cloudflare will give you a temporary `*.pages.dev` address to test.

## Connect your domain later

In Cloudflare Pages, open the project → **Custom domains** → **Set up a domain**. For a root/apex domain, Cloudflare requires the domain to be onboarded to Cloudflare DNS and its nameservers updated. Before changing nameservers at Network Solutions, review and preserve all existing DNS records, especially MX, TXT, and CNAME records used by email or other services. If you want to keep DNS at Network Solutions, you can instead use a subdomain such as `www` with the CNAME method supported by Cloudflare Pages, after adding that subdomain in the Pages dashboard.

Do not share your Network Solutions, GitHub, or Cloudflare passwords with anyone.

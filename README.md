# The Hive website launch kit

This package is ready for **GitHub + Netlify**.

It is designed to keep things simple:
- **GitHub** stores the website files
- **Netlify** hosts the website and gives you SSL/HTTPS automatically
- **Calendly** handles booking calls
- **Netlify Forms** handles contact messages

This version does **not** require a custom backend.

## What's included

- `index.html` — your homepage
- `styles.css` — all website styling
- `thanks.html` — the thank-you page after someone submits the form
- `netlify.toml` — Netlify settings and security headers
- `assets/thehive-logo.jpg` — your logo

## Before you launch

Open `index.html` and replace these two placeholders:

- `YOUR_CALENDLY_REX_URL`
- `YOUR_CALENDLY_RAFAEL_URL`

Example format:
- `https://calendly.com/rex-example/30min`
- `https://calendly.com/rafael-example/30min`

Also review:
- contact email address
- team descriptions
- services copy
- resources section

## The easiest way to launch

### Option 1: GitHub website upload (easiest)

1. Create a new GitHub repository.
2. Name it something like `thehive-website`.
3. Click **Add file** → **Upload files**.
4. Upload everything from this folder.
5. Commit the files.

### Option 2: GitHub Desktop

1. Install GitHub Desktop.
2. Create a new local repository.
3. Copy all files from this folder into that repository folder.
4. Commit the files.
5. Publish the repository to GitHub.

## Deploy on Netlify

1. Log in to Netlify.
2. Click **Add new site** or **Import an existing project**.
3. Choose **GitHub**.
4. Connect the repository you just created.
5. Keep the defaults and deploy.

Because this is a static site:
- there is no build command required
- the publish directory is the site root

## Set up the contact form

After the first deploy:

1. Open your site in Netlify.
2. Go to **Forms**.
3. Confirm Netlify detected the form named `contact`.
4. Add email notifications so submissions go to your inbox.
5. Submit a test message from the live site.

## Connect your domain

In Netlify:

1. Go to **Domain management**.
2. Add:
   - `thehive.consulting`
   - `www.thehive.consulting`
3. Follow Netlify's DNS instructions where your domain is registered.
4. Wait for SSL to finish provisioning.

## Security included

This starter includes security headers in `netlify.toml`, including:
- `X-Frame-Options`
- `X-Content-Type-Options`
- `Referrer-Policy`
- `Permissions-Policy`
- `Content-Security-Policy`

That gives you a strong default setup for a marketing site.

## How future edits will work

Your workflow can stay simple:

1. Ask AI to update your HTML, CSS, or copy.
2. Replace the files in your GitHub repo.
3. Commit the changes.
4. Netlify automatically publishes the update.

## Suggested next improvements after launch

- add real client testimonials
- add downloadable resources
- add Google Analytics or Plausible
- add a privacy policy page
- add a favicon and social sharing image
- add an email newsletter signup later if needed

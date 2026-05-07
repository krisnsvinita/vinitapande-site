# Your Website — vinitapande.com

Dear Vinita,

Inside this folder is the complete code for your new website. It's ready to deploy.

---

## What's Inside

```
vinitapande-site/
├── index.html              ← Homepage
├── return-of-the-rishis.html  ← New book page
├── books.html              ← All books
├── services.html           ← Spiritual services
├── about.html              ← Your bio
├── contact.html            ← Contact page
├── styles.css              ← Shared design system (one file controls all pages)
├── images/                 ← All images
└── README.md               ← This file
```

**6 pages, 1 stylesheet, 6 images.** Total size: ~1.1 MB.

---

## Two Things to Do Before Going Live

### 1. Set up your Google Form (10 minutes)

Your "Contact" button currently links to a placeholder. Set up a Google Form so visitors can reach you. See the separate file `Google-Form-Setup-Instructions.md` for step-by-step setup.

After creating the form, you'll need to update **two places** in the code:
- `index.html` (search for `YOUR_GOOGLE_FORM_LINK_HERE`)
- `contact.html` (same placeholder)

Replace both with your real form link. Claude Code can do this for you in seconds, just say: *"Replace YOUR_GOOGLE_FORM_LINK_HERE everywhere with [paste your Google Form link]."*

### 2. Verify your Amazon book links

On `return-of-the-rishis.html` and `books.html`, the Amazon US/India/UK buttons currently point to generic Amazon pages (since you mentioned you're updating these). Once your real Amazon listings go live, replace these placeholder URLs.

---

## How to Deploy

You have two paths. Pick whichever feels right.

### Path A: Drop straight into Claude Code (recommended)

1. Save this folder somewhere on your laptop (e.g., `~/Sites/vinitapande-site`)
2. Open Terminal and navigate inside the folder:
   ```bash
   cd ~/Sites/vinitapande-site
   ```
3. Initialize Git and connect to GitHub:
   ```bash
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin git@github.com:YOUR-USERNAME/vinitapande-site.git
   git push -u origin main
   ```
4. Go to **vercel.com/new**, import the repo, click Deploy
5. Connect your custom domain in Vercel settings
6. Update DNS at your domain registrar with the records Vercel provides

### Path B: Let Claude Code drive

Once you have Claude Code installed (see `Vinita-Setup-Guide.md`), simply:

1. Save the folder somewhere on your laptop
2. Open Terminal, navigate inside the folder
3. Run `claude`
4. Ask it: *"Help me push this site to GitHub and deploy to Vercel."*

Claude Code will walk you through it.

---

## How to Edit Going Forward

Once everything is live, daily edits are simple:

```bash
cd ~/Sites/vinitapande-site
claude
```

Then describe changes in natural language:
- *"Update the homepage to mention my upcoming podcast appearance"*
- *"Replace YOUR_GOOGLE_FORM_LINK_HERE everywhere with https://forms.gle/abc123"*
- *"Change the book release date from June 18 to June 25"*
- *"Add a new YouTube video to the Books page"*

After Claude makes changes:

```bash
git add .
git commit -m "what you changed"
git push
```

Vercel auto-deploys in 30 seconds.

---

## Design Notes

The site uses a unified design system across all pages:

- **Colors:** Deep burgundy + saffron + sacred gold + cream
- **Fonts:** Cormorant Garamond (headings) + Spectral (body) + Cormorant Unicase (eyebrows)
- **All pages share `styles.css`** so updating once propagates to all 6 pages

If you want a global change (like swapping the burgundy for a different shade), tell Claude Code: *"In styles.css, change the burgundy-deep variable from #4A1410 to [new color]"* and it cascades everywhere.

---

## What's NOT in This Code Yet

A few things were intentionally left out, to be added when ready:

1. **Your photo on the About page.** Currently bio-only. Send me a photo and we can add it.
2. **Real Amazon book listing URLs.** Placeholders in place.
3. **Google Form link.** See setup instructions.
4. **Blog integration.** Currently just links to your existing Blogspot. We can integrate later if you want it on-domain.
5. **Newsletter signup.** Not built. Easy to add when you're ready (MailerLite recommended).

---

## Backup

The original homepage (locked, untouched) is preserved separately at `index-LOCKED-BACKUP.html` in the working version. Don't include that file in production.

If anything ever goes wrong, GitHub keeps a complete history of every change. Reverting takes one command:
```bash
git revert HEAD
git push
```

---

## When You Need Help

- **Technical issues:** Reach out to Ragini, or describe the issue to Claude Code itself
- **Content updates:** Just open Claude Code and describe what you want
- **Design changes:** Same — Claude Code understands CSS

The launch target is before **May 18** to align with your eBook pre-order date.

With love,

Ragini & Claude

---

ॐ नमः शिवाय

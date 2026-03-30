# Whata Got Going — Website

Johnson County handyman website. One file, no build step, nothing to install.

---

## How to Put This on GitHub Pages (Free Hosting)

### Step 1 — Create a GitHub account
Go to https://github.com and sign up if you don't have one.
Use any username. It'll show in your URL, so something simple works (example: `brjones1985`).

### Step 2 — Create a new repository
1. Click the green **New** button (top left after you log in)
2. Name it: `whatagotgoing`
3. Set it to **Public**
4. Leave everything else alone
5. Click **Create repository**

### Step 3 — Upload the file
1. On the repo page, click **uploading an existing file** (the link in the middle of the page)
2. Drag `index.html` into the upload box
3. Scroll down, click **Commit changes**

### Step 4 — Turn on GitHub Pages
1. Click **Settings** (top menu of your repo)
2. Click **Pages** (left sidebar)
3. Under "Branch", change the dropdown from `None` to `main`
4. Click **Save**

### Step 5 — Your site is live
Wait about 60 seconds, then go to:
`https://YOUR-USERNAME.github.io/whatagotgoing`

That's it. It's live. Free forever.

---

## How to Add Real Photos

### Option A — Upload to GitHub (easiest)
1. Take photos on your phone, name them `photo1.jpg`, `photo2.jpg`, etc.
2. Go to your repo on GitHub
3. Click **Add file → Upload files**
4. Upload your photos
5. Open `index.html` in GitHub's editor (click the file, then the pencil icon)
6. Find this section near the gallery:

```html
<div class="gallery-slot" onclick="document.getElementById('photo-upload').click()">
  <div class="gallery-slot-icon">📷</div>
  <div class="gallery-slot-label">Add Photo</div>
</div>
```

Replace each slot with this (one per photo):

```html
<div class="gallery-slot">
  <img src="photo1.jpg" alt="Fence job, Johnson County" style="display:block" />
</div>
```

7. Commit the change. Done.

### Option B — Link from Facebook/Google Photos
If your photos are already on Facebook or Google Photos, you can right-click → Copy image address and use that URL as the `src`. Easier, but the link can break if you move the photo.

---

## How to Add Real Testimonials

Find the three placeholder blocks in `index.html` that look like this:

```html
<div class="testimonial-placeholder">
  ...Your first review goes here...
</div>
```

Replace each one with a real quote like this:

```html
<div class="testimonial-card">
  <div class="testimonial-stars">★★★★★</div>
  <div class="testimonial-text">"Built us a fence on short notice, showed up when he said he would, priced fair."</div>
  <div class="testimonial-name">— J. Smith, Clarksville</div>
</div>
```

Use the person's first name and town. That's enough — nobody expects a full name.

---

## How to Update Your Facebook Link

Find this in `index.html`:

```html
<a href="https://facebook.com" target="_blank" ...>
```

Replace `https://facebook.com` with the actual URL of your Facebook page.
Example: `https://www.facebook.com/whatagotgoing`

---

## How to Update the Site After Changes

1. Make your edits to `index.html`
2. Go to your repo on GitHub
3. Click `index.html` → pencil icon → paste in the new content
4. Click **Commit changes**

The site updates in about 30 seconds.

---

## One-Time FormSubmit Activation

The contact form sends to your Gmail. The first time someone submits it, FormSubmit will send you an activation email. Open it and click the confirm link. After that, every form submission goes straight to your inbox with no extra steps.

---

## Questions

(479) 774-2643 | flatbottom.brjones1985@gmail.com

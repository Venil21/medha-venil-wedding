# Medha & Venil — Wedding Website

A static, single-page wedding website. No backend, database, or server required —
it's plain HTML/CSS/JS and can be hosted for free on GitHub Pages.

## Files

```
index.html              the whole site
assets/couple-caricature.jpg   the caricature image shown on the hero + modal
```

## 1. Host it on GitHub Pages (free)

1. Create a new GitHub repository (e.g. `medha-venil-wedding`). It can be public or private
   (private repos need a paid plan for Pages — public is fine and totally normal for a wedding site).
2. Upload `index.html` and the `assets/` folder to the repo (drag-and-drop on github.com works,
   or `git add . && git commit -m "wedding site" && git push`).
3. In the repo, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Under **Branch**, choose `main` and folder `/ (root)`, then **Save**.
6. GitHub will give you a live URL after a minute or two, usually:
   `https://<your-username>.github.io/<repo-name>/`

That's it — the site is now live and free, and updates automatically whenever you push changes.

## 2. RSVP form → your email

The RSVP form uses **FormSubmit** (formsubmit.co), a free service that emails form
submissions straight to an inbox — no backend, sign-up, or API key needed. It's already
wired to send to **vidmedha@gmail.com**.

**One-time activation step:** the very first time anyone submits the RSVP form, FormSubmit
sends a confirmation email to vidmedha@gmail.com with a link that says something like
"Activate Form." Click that link once — after that, every future submission is delivered
straight to the inbox automatically. It's worth doing a test RSVP yourself right after
publishing the site so this activation happens before real guests start responding.

Each submission arrives as a nicely formatted email with the guest's name, side, events
attending, guest count, dietary notes, and message.

If you'd rather not depend on a third-party mailer, alternatives are:
- **Formspree** (formspree.io) — similar free service, requires a quick sign-up.
- A `mailto:` link instead of a form (opens the guest's own email app — simpler, but less seamless).

## 3. Customizing

- Wedding details, schedule, and copy are all in the sections inside `index.html` — search
  for the section headers (`OUR STORY`, `SCHEDULE`, `VENUE`, `RSVP`, etc).
- The caricature image can be swapped by replacing `assets/couple-caricature.jpg` with a
  new image of the same filename (or update the two `src="assets/couple-caricature.jpg"`
  references in `index.html`).
- Background flower doodles (lotus, rose, lily, marigold) are inline SVG patterns in the
  `<style>` block — search for `Parallax Doodles Backgrounds` to tweak colors or opacity.

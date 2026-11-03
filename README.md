# University Tech Society: Student Organization Website

> A 4-page static website for a fictional university tech society, built as our team project for the first-semester Introduction to ICT course: HTML, CSS, a little JavaScript and simulated sign-up forms.

**Status:** Completed course project (Dec 2025) · Team of 4; I wrote most of the code (33 of 39 commits)
**Demo:** [Live site](https://hamzakhanbuic.github.io/University-Tech-Society---Student-Organization-Website/)

## Pages

Home (`index.html`), Events (`pages/events.html`), Register (`pages/register.html`) and About (`pages/about.html`). The team and "get involved" parts are sections of the Home and About pages. There are no Contact or Team pages.

## Quickstart

No build step and no dependencies. Open `index.html` in a browser, or serve it locally:

```bash
git clone https://github.com/HamzaKhanBUIC/University-Tech-Society---Student-Organization-Website.git
cd University-Tech-Society---Student-Organization-Website
python -m http.server 8000
```

Then open http://localhost:8000.

## Configuration

None. The pages load Font Awesome and Google Fonts from CDNs (Bootstrap 5.3.0-alpha1 on the Register page only), plus a few Unsplash images, so they need an internet connection.

## Team

- **Hamza Imran**: HTML structure, core CSS, layout, form validation.
- **Saqib Shah**: JavaScript interactivity and deployment.
- **Shayan Ullah**: UI/UX design, CSS animations, color scheme.
- **Uzair Ali**: content writing, documentation, quality checks.

(Roles as listed on the About page for the course submission. Commit history: Hamza Imran 33, Saqib Shah 3, Shayan Ullah 3.)

## Limitations

- The forms are simulations. Submitting shows an alert and nothing is sent or stored.
- No tests, no linting.
- No favicon: every page links `images/favicon.ico`, which does not exist (404).
- About 23 links are `#` placeholders (for example the social icons).
- The event form writes the user's own input into the page with `innerHTML` (self-XSS only, nothing is stored or shared).
- Bootstrap on the Register page is a pre-release version (5.3.0-alpha1), and the CDN assets have no integrity hashes.
- About 40 MB of MP4 video is tracked in the repository.
- It is a course project and not a maintained site.

## License

MIT. See [LICENSE](LICENSE).

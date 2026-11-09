# Embassy Electricals: Landing Page

**Live site:** https://wachiramorris7-alt.github.io/Professional company landing page/
**Repository:** https://github.com/wachiramorris7-alt/Professional company landing page

A landing page for **Embassy Electricals**, a fictional electrical engineering company based in Kenya. The site presents the company's services and lets customers request work online through a single service request form.

> Embassy Electricals is a fictional company created for a web development course project. All details are made up for demonstration.

## Project brief

The client, Embassy Electricals, wants a professional web presence that:

- introduces the company with a clear promise: *"Wired right. Fixed fast."*
- explains how it works: fully online applications, cashless payment, 24-hour service and emergency priority
- lists the installations and services it offers
- lets customers submit a service request with their details, location, type of service and photos or video of the problem
- shows contact details, including an emergency hotline

## Business rationale

| Business goal | How the site supports it |
|---|---|
| Replace paper applications and queues | A single online form collects customer, location, service and power-source details |
| Speed up fault diagnosis | The form accepts a photo (required) and an optional video, so agents see the problem before dispatch |
| Build trust | The About section states the company's policies: free applications, quality assurance, traceable records in one e-file |
| Serve all customer types | The environment dropdown covers homes, apartments, industry, hotels/shops and hospitals |
| Handle urgent jobs | Emergencies are prioritised and a hotline number is shown in the contact block |

## Page sections

1. **Intro screen**: full-screen branded splash with the year.
2. **Hero**: value proposition ("Wired right. Fixed fast.") and welcome message.
3. **About the company**: service policies and the six main installation types (solar PV, low-voltage grid, high-voltage grid, isolator switches, motor winding/rewinding, consumer control panels).
4. **Services**: eight service areas (installation, restoration, risk assessment, risk mitigation, expert advisory, supervision, mapping and planning, recruitment) with a short description.
5. **Service request form**: name, ID/passport number, email, location, member status, environment, service type, power source, message, and photo/video uploads.
6. **Contact information**: phone numbers, hotline, WhatsApp and email.
7. **Footer**: company domain, tagline and year.

## Technologies used

- **HTML5**: page structure, forms, `section`, `header` and `footer` elements
- **CSS3**: external stylesheet, full-viewport background images, a media query for small screens
- **Git and GitHub**: version control
- **GitHub Pages**: hosting

No frameworks or build tools are used.

## Setup instructions

```bash
git clone https://github.com/wachiramorris7-alt/Professional company landing page
.git
cd Professional company landing page
```

Then open `index.html` in a browser, or run a local server:

```bash
python3 -m http.server 8000
# visit http://localhost:8000
```

### Deploy to GitHub Pages

1. Push the `main` branch to GitHub.
2. Go to **Settings > Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
4. The site is live after about a minute at the URL above.

## Project structure

```
.
├── index.html
├── style.css
├── assets/        background images used by the stylesheet
└── README.md
```

## Git workflow

The project uses feature-based branching:

- `main`: production branch, deployed to GitHub Pages
- `develop`: integration branch
- `feature/*`: one branch per piece of work, merged into `develop` and then into `main`

## Screenshots

| Desktop | Mobile |
|---|---|
| ![Desktop view](docs/screenshot-desktop.png) | ![Mobile view](docs/screenshot-mobile.png) |

## Known limitations and planned improvements

Being upfront about what is not finished yet:

- **Form backend:** the form posts to `/submit`, which does not exist on GitHub Pages  a small server, is needed to receive submissions.
- **Validation:** the form currently relies on the browser's built-in `required` checks. 
- **Navigation:** the page has no menu yet. (my intention was since its a service company a client must read thru all pages till the last one not just jump pages so i went for scroll down.)

- **Responsive design:** am not sure if all phones can comfotaply view
- **Social links:** the footer will get links to the company's social media pages.

## Credits

- Background photos from [Pexels](https://www.pexels.com/): Bence Szemerey, Rafael Carneiro and Michal Robak.
- Built by Morris mwaniki for software engineering, 2026.

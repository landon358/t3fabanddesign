# T3 Design & Fab — website

Static site for T3 Design & Fab, a welding and metal fabrication shop at
1255 Leonard St NW, Grand Rapids, MI 49504.

## Pages

| File | Page |
| --- | --- |
| `index.html` | Redirects to the home page |
| `Home.dc.html` | Home |
| `Wheel-Repair.dc.html` | Wheel & Rim Repair |
| `Aluminum-Welding.dc.html` | Aluminum & Specialty Welding |
| `Rust-Repair.dc.html` | Truck & Auto Rust Repair |
| `Custom-Fabrication.dc.html` | Custom Fabrication |
| `Design-Prototyping.dc.html` | Design & Prototyping (SolidWorks) |
| `About.dc.html` | About |
| `Contact.dc.html` | Contact & Quote |

Shared pieces: `SiteNav.dc.html` (sticky header, hamburger menu under 900px)
and `SiteFooter.dc.html` (collapsible sections under 760px). `support.js` is
the small runtime both rely on. Photography lives in `photos/`.

## Running it

It is plain static HTML — no build step.

```
python3 -m http.server 8000
```

then open http://localhost:8000

## GitHub Pages

Push to a repo and enable Pages on the branch root. `.nojekyll` is included so
every file is served as-is.

## Before going live

- Confirm the phone number: (616) 589-8594 is used throughout; (616) 666-4796
  is also in active use on Facebook and Yelp. Pick one and update all listings.
- Confirm hours. The site shows Mon–Sat 9a–8p, Sunday by appointment.
- Confirm an email address, ideally on the new domain rather than Yahoo.
- Replace the two portrait placeholders on the About page with real photos of
  Tom and Thomas, and add an exterior shot and a photo of the service truck.
- The contact form is front-end only — wire it to a form service (Formspree,
  Netlify Forms, or similar) or remove it in favour of call/text.
- State the mobile welding radius on Contact once it is confirmed.

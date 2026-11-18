# Casket Cafe — static website proposal

A multi-page, frontend-only website built with HTML, CSS, and vanilla JavaScript. It runs from static files and is suitable for GitHub Pages. The official logo supplied for this proposal is preserved at `assets/logo/casket-cafe-logo.png` and is used as provided.

The visual system combines UnifrakturCook and IM Fell English gothic display typography with orange, white, and black. The homepage uses subtle candlelight motion, arch framing, and animated ornaments; motion effects respect reduced-motion settings.

## Preview

Open `index.html` in a browser. No build step, package manager, or server is required. Site links use relative paths, so the project works from a repository subdirectory as well as a domain root. Some browsers may block Google Fonts when opening local files offline; system serif and sans-serif fallbacks are included.

## GitHub Pages deployment

1. Commit and push the project contents to a GitHub repository.
2. In repository **Settings → Pages**, choose **Deploy from a branch**, select the publishing branch and `/ (root)` folder, then save.
3. Once published, replace `YOUR-DOMAIN` in `sitemap.xml` and `robots.txt` with the Pages origin. For a project site, the URL includes the repository subdirectory, for example `https://OWNER.github.io/REPOSITORY/`.
4. Add verified business content and café-owned photography before public launch.

There is no backend, authentication, payment provider, email service, or reservation service in this project. Forms validate locally and show a demo notice. The cart, profile, favourites, and dashboard use browser LocalStorage and are not shared between devices. Never enter payment details into the demo.

## Editable content

- `js/menu-data.js`: menu records. Replace sample names, descriptions, prices (`price` as a number), dietary labels, availability, categories, and image paths. The records currently cover all requested categories and are explicit placeholders, not actual Casket Cafe products or prices.
- Page copy: edit the relevant `.html` page. Business address, phone, email, opening hours, policies, and testimonials are not fabricated.
- `admin/index.html`: public client-side dashboard demonstration. It is not secure; saved edits only affect that browser and do not publish content. A production admin requires a backend or secure CMS.
- `assets/images/`: illustrative images downloaded from Unsplash for this visual proposal. Replace these with approved café photography. The image filenames and markup identify their uses; keep local paths and update alt text when replacing them.
- Homepage video: streams from [Pexels, “Cozy Indoor Cafe with Autumn Decor and Brick Walls”](https://www.pexels.com/video/cozy-indoor-cafe-with-autumn-decor-and-brick-walls-29003319/) by Ellysa Jordens. Pexels lists the clip as free. The local café still is the poster/fallback; playback requires internet access.
- `assets/logo/`: supplied brand artwork. The original logo image is kept unchanged and reused for the favicon.

## Pages and interactions

Home, Our Story, Menu, Gallery, Experiences, Reservations, Contact, FAQ, Cart, Guest Book demo, Privacy, Terms, a separate admin demo, and a custom `404.html` are included. Menu filters/search/sort, favorites, cart quantities, gallery lightbox, FAQ accordions, reservation/contact form validation, and client-side admin demonstrations are implemented with vanilla JavaScript.

Before production, replace every placeholder, connect real reservation/contact/newsletter/order services, add a reviewed privacy policy and terms, and confirm all menu and business information. No tests or backend services are required to preview this static proposal.

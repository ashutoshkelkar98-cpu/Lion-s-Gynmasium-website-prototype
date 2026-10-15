# Lion’s Gymnasium website prototype

Four-page static website: Home, Packages, Gym Gallery, and Enquiry & Bookings.

## Cloudflare Pages

Connect this repository and select:
- Production branch: `main`
- Framework preset: None
- Build command: leave blank
- Build output directory: `dist`
- Root directory: leave default

The committed `dist` folder is ready to deploy without installing dependencies. Future commits to `main` trigger deployment when Git integration is enabled.

## Cloudflare Workers (alternative)

The `wrangler.jsonc` file configures static assets from `dist`. In Workers Builds, leave the build command blank and use `npx wrangler deploy` as the deploy command.

## Local preview

Run `python3 -m http.server 8080 --directory dist` and open http://localhost:8080.

## Prototype limitations

Packages and images are illustrative. The enquiry form validates and previews an enquiry but sends and stores nothing. About Us, genuine testimonials, and Location & Contact are planned. Replace stock images, confirm membership details, and add a live enquiry integration before launch.

Edit the HTML in `dist` and shared styling/behaviour in `dist/assets`.

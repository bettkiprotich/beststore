# Beest Athletic demo

A responsive static website with a featured jersey kit, custom order enquiry through WhatsApp, and location guidance. All content is in `dist/`; open `dist/index.html` locally or serve `dist/` with any static web server.

## Update content

Edit `dist/business.js` to change the phone number, listed address, product data, and verified social links. The featured image is `dist/assets/psalms-105-kit.png`. The logo is displayed from the supplied business profile screenshot at `dist/assets/beest-profile.png` using the circular crop styling in `dist/style.css` (`.logo-crop`). For the best production result, replace that screenshot with an official transparent or high resolution logo and update the logo markup and favicon in `dist/index.html`.

## Exact location

The map currently searches the listed address rather than marking a verified shop entrance. Once Beest confirms the pin, set `exactMapPin` in `dist/business.js` to its official Google Maps URL. The address and `directionsQuery` can be updated there too. Consider replacing the embedded map search with the official place embed when the pin is confirmed.

## Deploy to Vercel

Import the project as a static site and set the output directory to `dist` with no build command. Alternatively run `npx vercel --prod` from this directory, with output directory `dist` configured in the Vercel project. No backend or secret keys are required.

The enquiry form opens WhatsApp with a composed message; it does not store or transmit customer data through this website.

# STREET — Drop 001 storefront

A responsive, dependency-free storefront for the STREET clothing brand.

## Preview locally

Open `index.html` in a modern browser. All imagery is stored in `assets/` and loaded with relative paths. For a local web server, run `python -m http.server 8000` in this folder and visit `http://localhost:8000`.

## Deploy to Vercel

1. Upload the **contents** of this folder to the root of a GitHub repository. Keep `index.html` and the `assets/` folder together.
2. Import the repository in Vercel.
3. Select **Other** as the framework preset. No build command is required; set the output directory to `.`.
4. Deploy.

The included `vercel.json` applies clean URL handling and basic security headers.

## Before taking real orders

- Replace the sample prices in the `products` array near the bottom of `index.html` with confirmed prices.
- Confirm product materials, fit, sizing, stock, and delivery terms. Product visuals for the jacket, tee, pants, boxer briefs, socks, and cap are concept mock-ups; replace them with final product photos before selling.
- Add your actual customer-service email, business details, privacy policy, terms, and return policy.
- Connect a real payment and order system (such as a hosted checkout provider). The bag and quantity controls work locally in the browser, but payment, order processing, stock, delivery, and newsletter collection are not connected.
- Add an accurate size chart and shipping cost / delivery information.

## Editing products

In `index.html`, find `const products = [...]`. Each product has an `id`, `name`, `category`, `price` (DKK), `label`, `image`, `gallery`, `sizes`, and `description`. Images are stored under `assets/`.

# Willie AI

A static landing page for the Willie AI new-parent assistant, powered by the CX Agent Studio web widget.

## Deploy to Vercel

1. Upload the contents of this `chatbot` folder to a GitHub repository, or set this folder as the Vercel project's **Root Directory** if the repository contains other folders.
2. Import the GitHub repository in Vercel.
3. Use the **Other** framework preset. No build command or install command is needed; leave them blank. Set the output directory to `.`.
4. Deploy. Vercel serves `index.html` as the site homepage.

## Connect the agent

The page is already configured for this CX Agent Studio deployment:

`projects/286851988515/locations/us/apps/fa6bd9ca-1cba-437a-b89c-858680a583d5/deployments/547cd575-e74e-4554-9c13-326eb5a8fb5b`

The widget title is **Willie AI**. The token broker and reCAPTCHA options are enabled, matching the supplied embed configuration. In CX Agent Studio, make sure the deployment's public access and token broker settings are enabled. After Vercel gives you a domain, add that production origin to the deployment's allowed origins if you configured an origin allowlist. For a custom domain, add that origin too.

The widget's `url-allowlist="*"` allows image URLs from any origin, matching the supplied snippet. To restrict images later, replace `*` with a comma-separated list of trusted origins.

## Local preview

Open `index.html` directly in a browser, or serve this folder with any static file server. The live chat requires an internet connection and a correctly configured CX Agent Studio deployment.

# Appliance Solutions Cloudflare website

Deploy the `public` directory using Cloudflare Pages. For Git deployment: framework preset None, build command `exit 0`, output directory `public`. Add `appliance-solutions.co.za` under Workers & Pages > project > Custom domains.

This is configured for https://appliance-solutions.co.za/. I cannot access your Cloudflare/registrar account to connect it directly. For the apex domain, add the domain as a Cloudflare zone and follow its nameserver instructions; preserve existing DNS records needed for email.

The quote form validates the fields and opens WhatsApp with the enquiry pre-filled. It does not claim to email or permanently store leads; the visitor must press Send in WhatsApp. `generate_lead` tracks form submission intent, not confirmed delivery. Tracking events include `generate_lead`, `phone_click`, `whatsapp_click`, and `quote_cta`. Replace `G-XXXXXXXXXX` in `public/index.html` with your GA4 Measurement ID, then configure relevant events as key events in GA4. Cloudflare Web Analytics can also be enabled in the Pages dashboard.

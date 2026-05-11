## Cursor Cloud specific instructions

This is a single static HTML landing page (`index.html`) with no build tools, package managers, or backend services.

### Running the dev server

Serve with any static HTTP server. The simplest option:

```
python3 -m http.server 8080 --directory /workspace
```

Then open `http://localhost:8080/index.html` in the browser.

### Notes

- There are no dependencies to install, no lint tools, no test frameworks, and no build step.
- The page embeds an external GoHighLevel form via iframe (`link.actionpotential.ai`). This is a third-party SaaS service and requires internet access to load.
- The page includes a 10-minute countdown timer (JavaScript) that starts on page load and disables the CTA when it expires.
- URL query parameters (`email`, `phone`, `name`, `contact_id`) are used to pre-fill the embedded form.

# Complete UI Development Prompt - ExampleOrg Code Reviewer

Build a simple custom UI for a generic GitHub Code Reviewer Agent called **ExampleOrg Code Reviewer**. Make it look like a practical project created by someone with basic HTML, CSS and JavaScript knowledge. Do not use a real company name or proprietary logo.

Use a simple white, light grey and blue colour scheme. Use normal readable fonts, basic borders, simple buttons and small spacing. Build with plain HTML, CSS, and JavaScript without Bootstrap or Tailwind. Avoid gradients, glass effects, glowing effects, complex animations, exaggerated marketing language, and decorative AI graphics.

The page must include a professional header with an ExampleOrg text mark, product title, n8n connection status, a short product introduction, repository input, pull request input, code-diff textarea, review button, review output panel, trust signals, responsive mobile layout, and footer.

Connect the form to `POST /webhook/github-code-reviewer` with this JSON payload:

```json
{"repository":"example-org/platform-service","pullRequest":"2481","codeDiff":"diff --git ..."}
```

The workflow returns `{ "review": "..." }`. Also accept `text`, `output`, or `data.review` response shapes. Keep the endpoint in one JavaScript constant.

Required states: validate all required fields, show loading and disable controls, show formatted findings on success, show a clear error on HTTP/network failure, preserve values for retry, and safely escape response text before formatting headings, bold text, and bullet lists.

Use visible focus states, accessible labels, `aria-live` messaging, and a simple loading message. Test desktop, tablet, mobile, validation, loading, success, and failure behavior.

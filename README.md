# RTI Application Text Validator & Fixer

A lightweight, single-page web utility designed to scrub forbidden characters from text drafts before submitting them to the Indian RTI Online portal (`rtionline.gov.in`). 

The official RTI portal frequently rejects text inputs with a generic error if any unauthorized punctuation marks or special characters are detected. This tool automatically scans your draft, highlights the offending characters, and provides a sanitized, copy-paste-ready version instantly.

## 🚀 Features

- **Strict Validation:** Automatically validates text against the exact character whitelist permitted by the RTI portal's backend.
- **Visual Error Tracking:** Isolates and displays the exact prohibited characters found in your draft (e.g., smart quotes, semicolons, apostrophes).
- **Instant Fixer:** Generates a cleaned version of your text with illegal characters stripped out, preserving formatting and allowed punctuation.
- **Privacy First:** Runs entirely in the browser (client-side JavaScript). Your data never leaves your machine and is never sent to a server.

## 📜 The RTI Character Whitelist

The RTI Online portal only permits the following characters:
- **Alphabets:** `A-Z` and `a-z`
- **Numbers:** `0-9`
- **Spaces & Newlines**
- **Special Characters:** `,` `.` `-` `_` `(` `)` `/` `@` `:` `&` `\` `?` `%`

*Note: Common culprits like apostrophes (`'`), quotation marks (`"`), semicolons (`;`), and exclamation marks (`!`) will trigger errors on the official portal and are caught by this utility.*

## 💻 Local Setup

Since this project consists of standard HTML, CSS, and vanilla JavaScript, it requires no installation, compilers, or local servers.

1. Clone or download this directory.
2. Rename your main application file to `index.html`.
3. Double-click `index.html` to run it locally in any modern web browser (Chrome, Firefox, Edge, Safari).

## 🌐 Deployment to Cloudflare Pages

This project is fully optimized for static hosting on **Cloudflare Pages** (Free Tier):

### Option 1: Direct Upload (Fastest)
1. Ensure your primary file is named `index.html` and placed inside a dedicated folder.
2. Log in to the Cloudflare Dashboard and navigate to **Workers & Pages**.
3. Click **Create application** -> **Pages** -> **Upload assets**.
4. Name your project, drag and drop the folder, and hit **Deploy site**.

### Option 2: Git Integration (Continuous Deployment)
1. Push this project folder to a GitHub or GitLab repository.
2. In the Cloudflare Dashboard, go to **Workers & Pages** -> **Create application** -> **Pages** -> **Connect to Git**.
3. Select your repository.
4. Set the **Framework preset** to `None`, leave the build command blank, and click **Save and Deploy**. Any future pushes to your repository will automatically update the live site.

## 📄 License
This utility is open-source and free to use for navigating public records requests.

# Chandana High School & College — Website Wrapper

An unofficial, lightweight landing page for **Chandana High School & College** in Chandana Chowrasta, Gazipur, Bangladesh. The page displays the institution's existing NetiCMS website inside a full-screen iframe and adds a floating email contact shortcut.

> **Note:** This repository is an independent website wrapper. It is not the institution's official website and is not affiliated with or endorsed by the institution.

## Live Website

[Open Chandana Website](https://foysalahmmedsadin.github.io/chandana/)

## Features

- Full-screen embedded view of the institution's NetiCMS website.
- Loading screen with an animated spinner while the embedded page loads.
- Floating email shortcut that opens the visitor's default email application.
- Responsive viewport layout for desktop and mobile browsers.
- Custom page title, description, social-sharing metadata, and favicon.
- Lightweight implementation with plain HTML, CSS, and JavaScript.

## Website Content Source

The page embeds the following external website:

[Chandana High School & College on NetiCMS](https://www.neticms.com/chandanahighschoolandcollege)

The institution's page content is hosted externally and is not stored in this repository. The embedded page must remain online and allow iframe embedding for the main content to display correctly.

## Contact

The floating email button opens a new message addressed to:

`foysal24x7@gmail.com`

This uses the browser's `mailto:` handler. The visitor needs a configured email application or webmail handler for it to work.

## Run Locally

1. Clone the repository:

   ```bash
   git clone https://github.com/FoysalAhmmedSadin/chandana.git
   ```

2. Open the project folder.
3. Open `index.html` in a modern web browser.

No package installation, build tools, or backend server are required.

## Project Structure

```
chandana/
├── index.html  # Page layout, styles, iframe, and email-button logic
├── a.png       # Favicon
└── README.md   # Project documentation
```

## Customization

You can customize the page by editing `index.html`:

- Change the embedded website by updating the iframe's `src` URL.
- Change the contact destination by editing the `mailto:` address.
- Update the page title and metadata in the `<head>` section.
- Adjust the loading screen and email button styles in the CSS.

Keep `a.png` in the repository root if you want to retain the current favicon.

## Deployment

This is a static website and can be hosted on GitHub Pages or another static hosting provider.

For GitHub Pages:

1. Open the repository's **Settings**.
2. Select **Pages**.
3. Choose the branch containing the website (usually `main`) and the root folder.
4. Save the settings and wait for deployment.

## Limitations

- The embedded website's availability, content, and performance depend on NetiCMS.
- Some websites block iframe embedding through their security policies. If that happens, the embedded content may not load.
- The loading overlay is hidden when the iframe fires its load event; that event does not guarantee every resource inside the external page has finished loading.
- The email shortcut opens the visitor's email handler; it does not send an email automatically.
- No backend, database, or automated test suite is included.

## Author

**Foysal Ahmmed Sadin**

- GitHub: [@FoysalAhmmedSadin](https://github.com/FoysalAhmmedSadin)
- Repository: [chandana](https://github.com/FoysalAhmmedSadin/chandana)

## License

No license file was found in this repository during documentation review. Unless a license is added, others do not automatically receive permission to reuse, modify, or redistribute this project's code.

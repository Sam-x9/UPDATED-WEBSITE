# Six-page IT Portfolio

A complete static website for GitHub Pages. No installation, build step, framework, CDN, or paid domain is required. All styles, scripts, and example images are included. The sample content is editable; review every personal claim before publishing.

## Files

- `index.html` — Home: introduction, strengths, explore cards, principles carousel
- `about.html` — biography, values, skills
- `media.html` — photo, project image, optional video instructions
- `resume.html` — resume sections and Print / Save as PDF button
- `projects.html` — four editable project examples
- `contact.html` — email and profile details
- `style.css` — shared styling, responsive layout, print styles
- `script.js` — mobile menu, carousel, print button, current year
- `assets/` — local placeholder images and favicon
- `.nojekyll` — static publishing marker

## Start here

1. Extract this ZIP.
2. Open `index.html` in your browser. Follow the navigation to see all six pages.
3. Open the HTML files in VS Code or any plain text editor.
4. Search for `EDIT` comments. Replace the example text with your information.
5. Save, then refresh your browser.

The pages contain normal HTML, so the content and navigation work without JavaScript. JavaScript adds the mobile menu, carousel, current year, and print button.

## What to replace

| Item | Where to edit |
| --- | --- |
| Your Name | Home introduction and footer on all six pages |
| My IT Portfolio | Title, header, and footer on all six pages |
| Biography and skills | about.html |
| Education and work experience | resume.html |
| Project descriptions | projects.html |
| Email | BOTH the `mailto:` address and visible text in contact.html |
| LinkedIn and GitHub | Replace the paragraphs using the commented examples in contact.html |
| Portrait | Add assets/profile.jpg, then change the image source in index.html and media.html; write useful alt text |
| Project image or certificate | Add your file to assets/ and update media.html, including alt text and caption |
| Resume PDF | Add assets/resume.pdf and uncomment the download link in resume.html |
| Video | Add assets/demo.mp4 and uncomment the video example in media.html |
| Colors | Variables at the beginning of style.css |
| Carousel text | principles array in script.js |

Keep filenames lowercase and match capitalization exactly. Use relative links such as `assets/profile.jpg`, not `/assets/profile.jpg`, so the site works within a repository URL. Do not rename the six HTML files unless you also update every link to them. The navigation and footer are repeated in each page so editing does not require a generator.

The included portrait and project images are placeholders. The resume has no active PDF download until you add a real PDF; its print button lets you save the visible resume as PDF through your browser. The contact email is an example and must be replaced. GitHub Pages hosts static files; the email link opens the visitor's email app, and there is no contact form backend.

## Publish on GitHub Pages

1. Sign in to GitHub and create a public repository, for example `it-portfolio`.
2. In the repository, choose **Add file → Upload files**.
3. Upload the CONTENTS of the extracted `portfolio` folder, including the `assets` folder. Do not upload just the ZIP or place the whole site inside another `portfolio` directory. `index.html` must be at the repository root.
4. Commit the uploaded files to your default branch, usually `main`.
5. Open **Settings → Pages**.
6. Under **Build and deployment**, select **Deploy from a branch**.
7. Select your branch (`main`) and **/ (root)**, then save.
8. Wait for GitHub to finish publishing and use the website URL shown on that Pages screen.

A project repository normally has a URL like `https://YOUR-USERNAME.github.io/it-portfolio/`. A repository named exactly `YOUR-USERNAME.github.io` uses `https://YOUR-USERNAME.github.io/` instead. Replace YOUR-USERNAME with your actual GitHub username.

For later changes, edit or upload the changed files and commit them. GitHub Pages republishes the site. You do not need a custom domain.

Official guide: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site

## Before publishing

- Replace all example identity and contact details.
- Review your biography, skills, dates, education, and experience for accuracy.
- Add only certificates you actually hold and projects you can explain.
- Check every page and link on both a narrow and wide screen.
- Avoid putting private addresses, credentials, or sensitive documents in the repository.

## Travel gallery customization

Media has five illustrated photo placeholders (not real destinations). Replace assets/travel-01.svg through assets/travel-05.svg with your photos. For JPG files, update each corresponding src in media.html to assets/travel-01.jpg, etc. Update the alt description, caption title, category, and location for each photo. The layout includes wide and portrait frames; use object-position on an individual image if its subject needs repositioning.

## Resume PDF

The Resume page includes a generated assets/resume.pdf based on the supplied resume. Open Resume PDF uses target="_blank"; browser PDF settings may open a viewer or download the file. Download PDF saves a copy directly. Replace assets/resume.pdf to update the document, and separately update resume.html to keep the website text in sync.

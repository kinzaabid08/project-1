# Sitemap & URL Structure

This document outlines the URL structure for the "Physical AI & Humanoid Robotics" website and provides instructions for publishing it via GitHub Pages.

## 🔗 Website URLs

The website uses clean, human-readable URLs that are compatible with static site generators and modern web standards.

-   **Homepage**: `/`
-   **Book Landing Page**: `/book/`
-   **Chapter 1**: `/book/the-rise-of-physical-ai`
-   **Chapter 2**: `/book/building-intelligent-robots`
-   **Chapter 3**: `/book/humanoid-robots-future`

---

## 🚀 Live URL Generation & Publishing

You can host this website for free using GitHub Pages.

### Example Live URLs

Once published, your URLs will look like this:

-   `https://your-username.github.io/your-project-name/`
-   `https://your-username.github.io/your-project-name/book/`
-   `https://your-username.github.io/your-project-name/book/the-rise-of-physical-ai`
-   `https://your-username.github.io/your-project-name/book/building-intelligent-robots`
-   `https://your-username.github.io/your-project-name/book/humanoid-robots-future`

### How to Publish on GitHub Pages (3 Steps)

1.  **Push to GitHub**:
    -   Create a new public repository on GitHub.
    -   Push your project files (`website` folder, `README.md`, etc.) to the `main` branch.

2.  **Enable GitHub Pages**:
    -   In your repository's **Settings**, go to the **Pages** tab.
    -   Under "Build and deployment," set the **Source** to **Deploy from a branch**.
    -   Set the **Branch** to `main` and the folder to `/ (root)`.
    -   Click **Save**.

3.  **Use a Static Site Generator (Recommended)**:
    -   For the URLs to work correctly without file extensions (e.g., `/book/` instead of `/book/index.html`), it's best to use a static site generator like **Jekyll**, **Hugo**, or **Docsify**.
    -   **Docsify Quick Start**: You can get a beautiful, functional site in minutes. Just create an `index.html` in your root directory with the following content, and Docsify will automatically build a single-page app with sidebar navigation from your Markdown files.

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
      <meta charset="UTF-8">
      <title>Physical AI & Humanoid Robotics</title>
      <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
      <meta name="description" content="A premium learning experience for Physical AI and Humanoid Robotics.">
      <meta name="viewport" content="width=device-width, initial-scale=1.0, minimum-scale=1.0">
      <link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify@4/lib/themes/vue.css">
    </head>
    <body>
      <div id="app"></div>
      <script>
        window.$docsify = {
          name: 'Physical AI & Humanoid Robotics',
          repo: 'your-username/your-project-name',
          loadSidebar: true,
          subMaxLevel: 2,
          alias: {
            '/.*/_sidebar.md': '/_sidebar.md'
          }
        }
      </script>
      <!-- Docsify v4 -->
      <script src="//cdn.jsdelivr.net/npm/docsify@4"></script>
    </body>
    </html>
    ```
    - You would also need to create a `_sidebar.md` file to define your navigation.

# How to use the Audible Library Extractor Chrome extension to extract your Audible library, publish it as a website on GitHub Pages, and then update it later by re-running the extractor

## 📦 1. Install & Run the Extension

1. **Add Audible Library Extractor to Chrome** from the Chrome Web Store. It adds a button to the Audible library page. ([Chrome Web Store][1])
2. **Open your Audible library** in the browser. ([Joonas Paakko][2])
3. **Click the “Audible Library Extractor” button** (near the search bar). ([Chrome Web Store][1])
4. In the extractor UI, choose what to extract (library, collections, wishlist) and start extraction. ([Joonas Paakko][2])
5. After extraction completes, the extension opens a **local gallery page** showing your Audible library. ([Joonas Paakko][2])

> The gallery is a snapshot of your current library — it doesn’t auto-update on its own. To refresh it later, you’ll need to run the extraction again.

---

## 🌐 2. Save a Standalone Gallery

- From the gallery page, use the extension’s menu “**Extension tools → Save standalone gallery**” to **download a ZIP** of the static website.

---

## 📤 3. Upload the Gallery to GitHub

Follow the **Uploading to GitHub** steps:

1. **Create a GitHub account** (if you don’t have one).
2. **Download and install GitHub Desktop** for easy repo management.
3. **Create a new local repository** (e.g., `my-audible-library`).
4. **Extract the standalone gallery ZIP**, move its files into your local repo folder.
5. In GitHub Desktop, **commit and publish** the repo to GitHub, making it **public**.
6. In the repo settings on github.com, **enable GitHub Pages** (select the `main` branch).

Your gallery is now hosted at a URL like:

```plain
https://YOUR-USERNAME.github.io/YOUR-REPOSITORY-NAME
```

---

## 🔄 4. Updating Your Gallery on GitHub

When your Audible library changes (new books, progress, etc.):

1. **Run Audible Library Extractor again** on Audible to fetch updated data.
2. **Save a fresh standalone gallery ZIP** via the extension.
3. In your GitHub Desktop project folder, **replace all old gallery files** with the new ones.
4. **Commit the changes**, then **push** (`Push origin`) back to GitHub.

GitHub Pages will rebuild the site with updated content.

---

## 📌 Notes

- The extractor creates **static content**, so any update requires a new extraction & upload.
- You don’t need to edit any code — just manage files with GitHub Desktop or the GitHub UI.

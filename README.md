 🌿 Icy Liu — Personal Website

> 刘宸瑜的个人网站 · Built with pure HTML/CSS/JS · No frameworks

 🔗 Live Site

https://liuchenyu1209.github.io/Individual-web_icy/

---

 📁 Project Structure

```
index.html        # 唯一文件，所有内容、样式、图片均内嵌其中
README.md         # 本文件
```

This is a single-file website — all images are base64-encoded directly into `index.html`, so no extra assets or build steps are needed.

---

 ✨ Sections

|   | Section | Content |
|---|---------|---------|
| — | Hero | Name, photo, links, tags, stats |
| 01 | Education | CityU HK (MSc) · HZNU (BSc) |
| 02 | Internship | User research · AI trainer |
| 03 | Research | 4 projects, conference papers |
| 04 | Skills | SPSS · JASP · MySQL · Cursor · VS Code… |
| 05 | Campus | 科协宣传 · 志愿服务 425h |
| 06 | Photography | Draggable horizontal photo strip |
| 07 | Life | Cycling · Hiking · Photography |
| 08 | About | Personal bio |
| — | Contact | Email · LinkedIn · Phone · 抖音 · 小红书 |

---

 🛠 How to Customize

 Update contact links
Search for the following placeholders in `index.html` and replace:

```
你的抖音链接        →  your Douyin profile URL
你的小红书链接      →  your Xiaohongshu profile URL
CV_LINK            →  your CV / resume URL
```

 Update the About section
Find the `about-placeholder` div and replace its content with your own text.

 Add new photos to work/research sections
Each expandable card has upload slots — click the `+` boxes directly in the browser to upload images locally.  
To permanently embed photos, replace the `<img>` `src` attribute with a base64 string (use the same Python script pattern used during build).

 Change your avatar
The hero avatar is the `生活照__1_` image, encoded inline. To swap it, encode your new photo to base64 and replace the `src` value on the `.hero-avatar` `<img>` tag.

---

 🚀 Deployment (GitHub Pages — Free)

1. Create a GitHub repository named `your-username.github.io`
2. Upload `index.html` (and this `README.md`) to the root
3. Go to Settings → Pages → Source → Deploy from branch (main)
4. Your site will be live at `https://your-username.github.io` within ~1 minute

No build step. No npm. No config. Just upload and go.

---

 🧰 Tech Stack

| Tool | Role |
|------|------|
| HTML5 / CSS3 | Structure & styling |
| Vanilla JS | Interactions (cursor, drag strip, lightbox, count-up, scroll reveal) |
| Google Fonts | Unbounded · Space Grotesk · Noto Sans SC |
| Python + Pillow | Image compression & base64 encoding (build-time only) |
| GitHub Pages | Hosting |

---

 📝 Notes

- All images are compressed to ≤900px wide at quality 72 before encoding, keeping the file around 3–4 MB
- Dark mode is supported via `prefers-color-scheme`
- The site is mobile-responsive (breakpoint at 900px)
- Custom cursor is desktop-only (hidden on touch devices automatically)

---

 👤 About

Made by 刘宸瑜 (Icy Liu)
MA Applied Social Science · City University of Hong Kong  
📧 liuchenyu1209@gmail.com  
💼 [LinkedIn](https://linkedin.com/in/chenyu-liu-3753b0341)

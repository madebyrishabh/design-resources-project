# Design Research Resources Project

A collection of open-access, searchable databases for design researchers — built using HTML, CSS, and JavaScript.

## 📂 Overview

This project includes two resources on [https://resources.rishabhpandey.com/](https://resources.rishabhpandey.com/):

1. **Design Journals Database** → [https://resources.rishabhpandey.com/journallist.html](https://resources.rishabhpandey.com/journallist.html)  
2. **Design Conferences Database** → [https://resources.rishabhpandey.com/conflist.html](https://resources.rishabhpandey.com/conflist.html)

These databases aim to make it easier for design researchers, educators, and students to find suitable venues for publication and collaboration.

## 🚀 Features

- Tag filters (HCI, XR, Communication, Industrial, Sustainability, etc.)
- Search by journal or conference title
- Multi-domain tagging (items can belong to multiple domains)
- Table header with sorting option
- Theme toggle (light and dark)
- Like button with counter (anonymous; one count per browser per 24h)
- Visitor counter (anonymous; one count per browser per 24h)

## 🧱 Tech

- HTML, CSS, JS
- Firebase Realtime Database (public counters only)
- Google Analytics (gtag)
- No build step required

## 🛠️ Project Structure

```
/assets                  # icons, images
/css                     # stylesheets
/js                      # scripts (table, filters, theme, UI)
├── script.js            
├── script_conf.js
├── script_journal.js
├── script_theme.js
index.html              # landing or redirect
conflist.html           # Design Conferences Database (uses its Firebase project)
journallist.html        # Design Journals Database (uses its Firebase project)
robots.txt              # crawl rules
sitemap.xml             # sitemap for search engines
```

##  🔐 Analytics & Privacy

- Google Analytics is used to collect aggregate usage insights to improve the site experience.
- The Firebase layer records only numeric counters for likes and page visits.
- No personally identifiable information (PII) is collected, stored, or shared.

##  🧩 Security

- All Firebase configuration files are excluded from version control and remain local.
- Firebase rules restrict data writes to controlled increments (+1 only).  
- Each counter is anonymous and stored as an aggregate number only.

##  🙌 Contribute / Suggest additions

This project grows with the community. You can:
- Open a GitHub Issue (bug/feature/data update), or
- Use the suggestion forms linked on the live pages to add journals/conferences.

Special thanks to **Swati Pandey** and **Akanksha Bhardwaj** for their assistance with data curation and feedback.

## ⚖️ License

Licensed under the **MIT License**.  
© 2025 Rishabh Pandey

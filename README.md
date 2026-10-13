# App Policies

Public privacy policies, account deletion pages and child safety standards for the mobile apps published by **Shrishu Innovations Private Limited**.

This repository is served as a static website using GitHub Pages. Each app has its own folder with its own privacy policy and account deletion page, plus a child safety standards page where Google Play requires one, so every page describes only the app it belongs to.

## Apps

| App | Privacy policy | Account deletion | Child safety standards |
|---|---|---|---|
| Tether Us | `/tetherus/` | `/tetherus/delete-account/` | `/tetherus/child-safety/` |
| Employeable | `/employeable/` | Not yet published | Not required |

Paths are relative to the root of the published site.

## Repository structure

```
.
├── README.md
├── employeable/
│   └── index.html                 # Privacy policy
└── tetherus/
    ├── index.html                 # Privacy policy
    ├── delete-account/
    │   └── index.html             # Account deletion instructions
    └── child-safety/
        └── index.html             # Child safety standards (CSAE policy)
```

Each page is a single, self-contained `index.html` with no scripts, cookies, analytics or external trackers. Naming the file `index.html` lets GitHub Pages serve it at the folder URL (for example `/tetherus/`) without `.html` on the end.

## Adding a new app

1. Create a folder named after the app in lowercase with no spaces, for example `safespace/`.
2. Add `index.html` (privacy policy) and `delete-account/index.html` (account deletion) inside it.
3. If the app is listed in Google Play's Social or Dating category, also add `child-safety/index.html` (child safety standards). Google Play requires these apps to publish standards against child sexual abuse and exploitation (CSAE).
4. Write each page for that app only. The privacy policy must match what the app actually collects, the third-party services it uses, the permissions it requests, and the answers given in the Google Play Data safety form.
5. Commit and push to `main`. GitHub Pages republishes within a couple of minutes.
6. Add the app to the table above.

## Maintenance rules

- **Do not rename or move app folders.** The page URLs are registered in Google Play Console and linked from inside published apps. Changing them breaks those links.
- **Keep the repository public.** Google Play requires these URLs to be publicly accessible without login.
- **Update the "Last updated" date** at the top of a page whenever its content changes.
- **Update the policy before releasing a version** that adds a new SDK, permission, or kind of data collection, and update the Data safety form at the same time.
- **Keep the pages consistent.** If the deletion process changes, update both the deletion page and the retention section of the policy. If the child safety reporting process or contact changes, update the child safety page and the Play Console declaration.
- **Only claim what the app does.** For example, the in-app reporting line on a child safety page should be enabled only once the feature exists in a released build.

## Contact

Shrishu Innovations Private Limited
Email: shrishuinnovations@gmail.com

For privacy questions, data access or deletion requests, child safety concerns, or complaints about how an app handles personal data, write to the address above and name the app in the subject line.
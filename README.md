# App Policies

Public privacy policies and account deletion pages for the mobile apps published by **Shrishu Innovations Private Limited**.

This repository is served as a static website using GitHub Pages. Each app has its own folder, its own privacy policy, and its own account deletion page, so every policy describes only the app it belongs to.

## Apps

| App | Privacy policy | Account deletion |
|---|---|---|
| Tether Us | `/tetherus/` | `/tetherus/delete-account/` |

Paths are relative to the root of the published site.

## Repository structure

```
.
├── README.md
└── tetherus/
    ├── index.html                 # Privacy policy
    └── delete-account/
        └── index.html             # Account deletion instructions
```

Each page is a single, self-contained `index.html` with no scripts, cookies, analytics or external trackers. Naming the file `index.html` lets GitHub Pages serve it at the folder URL (for example `/tetherus/`) without `.html` on the end.

## Adding a new app

1. Create a folder named after the app in lowercase with no spaces, for example `safespace/`.
2. Add `index.html` (privacy policy) and `delete-account/index.html` (account deletion) inside it.
3. Write the policy for that app only. It must match what the app actually collects, the third-party services it uses, the permissions it requests, and the answers given in the Google Play Data safety form.
4. Commit and push to `main`. GitHub Pages republishes within a couple of minutes.
5. Add the app to the table above.

## Maintenance rules

- **Do not rename or move app folders.** The page URLs are registered in Google Play Console and linked from inside published apps. Changing them breaks those links.
- **Keep the repository public.** Google Play requires privacy policy URLs to be publicly accessible without login.
- **Update the "Last updated" date** at the top of a policy whenever its content changes.
- **Update the policy before releasing a version** that adds a new SDK, permission, or kind of data collection, and update the Data safety form at the same time.
- **Keep policy and deletion page consistent.** If the deletion process changes, update both the deletion page and the retention section of the policy.

## Contact

Shrishu Innovations Private Limited
Email: shrishuinnovations@gmail.com

For privacy questions, data access or deletion requests, or complaints about how an app handles personal data, write to the address above and name the app in the subject line.
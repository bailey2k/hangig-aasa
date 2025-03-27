# 🔗 Hangig Universal Links Setup

This repo hosts the `.well-known/apple-app-site-association` file for the [Hangig](https://hangig.app) iOS app.

It enables **Apple Universal Links**, allowing users to tap on invite links like:

```
https://hangig.app/invite?tripID=xyz123
```

...and automatically open the Hangig app.

---

## 📦 What’s Inside

- `.well-known/apple-app-site-association`  
  JSON file that registers Hangig's bundle ID with `/invite/*` URL paths

---

## 🛠 Hosted on Vercel

This repo is auto-deployed via [Vercel](https://vercel.com) and served at:

```
https://hangig.app/.well-known/apple-app-site-association
```

- ✅ Fast HTTPS hosting
- ✅ Proper `Content-Type: application/json` header
- ✅ Custom domain + AASA compliant

---

## 📱 Supported App ID

```json
{
  "appID": "YOUR_TEAM_ID.bailey2k.hangig",
  "paths": [ "/invite/*" ]
}
```

> Replace `YOUR_TEAM_ID` with your real Apple Developer Team ID (found in [developer.apple.com](https://developer.apple.com/account)).

---

## ✨ Purpose

This setup allows Hangig to:
- Onboard users via universal invite links
- Skip splash/login when users tap shared trip links
- Provide a seamless deep linking experience on iOS

---

## 💡 Bonus

Want to use your own domain for Universal Links?  
Here’s how this setup works:
- [Apple Universal Links Guide →](https://developer.apple.com/documentation/xcode/supporting-universal-links-in-your-app)
- [AASA file format →](https://developer.apple.com/documentation/safariservices/supporting_associated_domains)

---

## 🧑‍💻 Built With

- [Vercel](https://vercel.com) for hosting
- macOS Terminal + GitHub for versioning
- Apple Universal Links for deep linking

---

## 🔐 Security

This repo does **not** contain any sensitive data.  
The contents of the AASA file are **public by design**.

---

## 📬 Contact

Made by [@bailey2k](https://github.com/bailey2k) for the [Hangig](https://hangig.app) app 💜
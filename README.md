# 🚀 QuasarModernBanner

✨ A clean, modern, and highly customizable banner component for Quasar Framework. Perfect for showcasing announcements, promotions, or alerts in your Vue.js Vite applications.

---

## ❓ Purpose
Quasar's vanilla Banners align with the Google Material Design Guide style, but I have always personally found
it boring and uninteresting.

I have created this component to bring a more modern look to the applications I develop in Quasar.

This component will be actively improved over time.

---

## 📦 Installation

Install the package via npm:

```bash
npm i quasar-modern-banner
```

---

## 🛠️ Usage
1. Import the component into your Vue file:

```bash
import { QModernBanner } from 'q-modern-banner'
```
2. Use it in your template:

```bash
<QModernBanner
    title="Potential Issues Found!"
    subtitle="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor."
    icon="person"
    type="info"
/>
```

---

## 🎨 Props

| Prop     | Type   | Note                                        |  
|----------|--------|---------------------------------------------|
| title    | String | ---                                         |
| subtitle | String | ---                                         |
| icon     | String | Uses Google Material Icons (Quasar Default) |
| type     | String | Either use `info`, `error` or `success`     |

---

## 🖼️ Examples
![Image of Banner Examples](https://gcdnb.pbrd.co/images/wq8BNQg8Ncu7.png?o=1)

---

## 🤝 Contributions
Contributions are welcomed. If you'd like to improve this component, please follow these steps:
1. Fork the repo.
2. Create a new branch `git checkout -b feature/AmazingFeature`.
3. Commit your changes `git commit -m 'Add some AmazingFeature'`.
4. Pull to the branch `git push origin feature/AmazingFeature`.
5. Open a pull request.
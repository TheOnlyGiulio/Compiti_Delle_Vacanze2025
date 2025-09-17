````markdown
# 🎭 Scam Meme App

A fun **Next.js + React Three Fiber** meme project that simulates a "you just got hacked/scammed" experience.  
It includes a flashy 3D button, Matrix-style hacker console, and fake IP geolocation reveal.

---

## ✨ Features
- **Next.js 13+** (App Router or Pages Router)
- **React + Hooks** (`useState`, `useEffect`, `useRef`, `useMemo`)
- **3D Graphics with Three.js**
  - via **@react-three/fiber** and **@react-three/drei**
- **Matrix Rain Effect** with the Canvas 2D API
- **Geo Data Lookup**
  - Calls the public API [`https://ipapi.co/json/`](https://ipapi.co/json/)  
  - Returns your **IP address, city, and country**
- **Phases**
  1. Intro screen with scammy banners + 3D claim button  
  2. Hacker console with fake logs + Matrix rain  
  3. "Results" with fake reveal and meme ending  

---

## 📡 API Usage
The app fetches basic geolocation data from:

```http
GET https://ipapi.co/json/
````

Response example:

```json
{
  "ip": "203.0.113.42",
  "city": "Example City",
  "country_name": "Example Country"
}
```

---

## 🖥 Requirements

* **Node.js** ≥ 16
* **npm** (comes with Node.js)

Dependencies:

```bash
next react react-dom @react-three/fiber @react-three/drei three
```

---

## 🚀 Getting Started

### 1. Create a Next.js project

```bash
npx create-next-app scam-meme
cd scam-meme
```

### 2. Install dependencies

```bash
npm install @react-three/fiber @react-three/drei three
```

### 3. Add the code

* If using **App Router (Next.js 13+)**: put the code in `app/page.tsx`
* If using **Pages Router**: put the code in `pages/index.tsx`

### 4. Run in development

```bash
npm run dev
```

Open in browser: [http://localhost:3000](http://localhost:3000)

---

## ⚙️ Development Notes

* Purely **client-side app** — no backend required.
* Designed for **meme/demo purposes only**.
* The “hack” is completely fake (it just uses public IP API).
* Fun example of mixing **3D graphics + React + Next.js**.

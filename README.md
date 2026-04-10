# reststueck.de

Riot Grrrl–inspirierte Landing Page für Reststück.
Minimal, roh, visuell direkt.

---

## 🚀 Tech Stack

* Next.js (App Router)
* Vercel (Hosting & Deployment)

---

## 📦 Setup (lokal)

```bash
git clone https://github.com/agent-botde/reststueck.git
cd reststueck
npm install
npm run dev
```

App läuft dann auf:
http://localhost:3000

---

## 🚀 Deployment (Vercel)

### Option A – CLI

```bash
vercel deploy --prod
```

---

### Option B – Dashboard

1. Repo mit Vercel verbinden
2. Framework: Next.js (auto-detected)
3. Deploy klicken

---

## 🌐 Domain verbinden (reststueck.de)

Im Vercel Dashboard:

1. Project öffnen
2. **Settings → Domains**
3. `reststueck.de` hinzufügen

---

### DNS beim Domain-Provider setzen:

**Für Root-Domain (`reststueck.de`):**

```
Type: A
Value: 76.76.21.21
```

**Für www (`www.reststueck.de`):**

```
Type: CNAME
Value: cname.vercel-dns.com
```

---

## 🧩 Favicon

Empfohlene Platzierung (Next.js App Router):

```
/app/icon.ico
```

Alternativ:

```
/public/favicon.ico
```

Dann in `app/layout.tsx`:

```ts
export const metadata = {
  icons: {
    icon: "/favicon.ico",
  },
};
```

---

## ⚠️ Hinweise

* Nach Änderungen am Favicon: Browser-Cache leeren
* Vercel deployt automatisch bei Git Push (wenn verbunden)
* Nur ein `/app`-Ordner im Projekt verwenden

---

## 🧠 Kontext

Projekt ist Teil einer autodidaktischen KI- & Bau-Reise von Hannes.
Mehr: https://agent-bot.de

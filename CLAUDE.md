@AGENTS.md

# Crypto Trading Terminal

## Tujuan project
Project belajar + portofolio pribadi. Bukan produk production, gak ada user beneran.
- Ngikutin course YouTube: "Crypto Trading Terminal Course | Build a Real-Time Dashboard with WebSockets & Next.js"
  https://www.youtube.com/watch?v=-vsh_GxC-vg&list=PL6QREj8te1P56tahJwEbyDZNVAnCclTc4
- Target akhir: dashboard trading crypto real-time (harga live via WebSocket, chart, dll) yang layak dipajang di portofolio.

## Cara bantu gw
- Ini buat belajar: jelasin *kenapa*, bukan cuma kasih kode. Kalau ada konsep baru (WebSocket, server vs client component, hooks, dll), kasih penjelasan singkat.
- Kalau gw nanya soal bagian course, bantu gw paham dulu. Jangan langsung nulis ulang semuanya kecuali gw minta.
- Kalau cara di video udah outdated buat versi Next.js/React di project ini, kasih tau bedanya dan pakai cara yang bener buat versi sekarang.
- Jawab pakai bahasa Indonesia santai. Istilah teknis tetap bahasa Inggris.
- Keep it simple. Gak usah over-engineering (gak perlu test suite gede, CI, dll) kecuali gw minta.

## Stack
- Next.js 16 (App Router, Turbopack), React 19, TypeScript
- Tailwind CSS v4 (config via CSS `@import "tailwindcss"` di `app/globals.css`, bukan `tailwind.config.js`)
- ESLint 9 (flat config, `eslint.config.mjs`)
- Path alias: `@/*` → root project
- Gw pakai editor Antigravity (video pakai WebStorm). Jangan kasih instruksi yang spesifik WebStorm.

## Commands
- `npm run dev`: dev server (http://localhost:3000)
- `npm run build`: production build (pakai buat ngecek error)
- `npm run lint`: lint

## Catatan
- Nama package `crypto-app`, bukan `crypto`, karena `crypto` itu nama core module Node dan ditolak npm.
- API key (kalau nanti ada) taruh di `.env.local`, jangan di-commit.

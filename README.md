<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:050505,55:1c1d20,100:0c63e7&height=170&section=header&text=StoreIt&fontSize=52&fontColor=fcfaf8&fontAlignY=38&desc=Cloud%20storage%20and%20file%20sharing&descAlignY=60&descSize=16" width="100%" alt="StoreIt" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" alt="Next.js" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Appwrite-FD366E?style=for-the-badge&logo=appwrite&logoColor=white" alt="Appwrite" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind CSS" />
  <img src="https://img.shields.io/badge/shadcn%2Fui-1c1d20?style=for-the-badge" alt="shadcn/ui" />
</p>

## ✨ About

StoreIt is a Google Drive–style storage platform. You can upload, organize, preview, share and manage files from one dashboard. It's built with **Next.js 15 server actions** and **Appwrite** for auth, database and file storage.

## 🔋 Features

- 🔐 **Passwordless auth**: sign up and sign in with an email one-time password (OTP)
- 📤 **Drag-and-drop uploads** with react-dropzone
- 🗂️ **Auto-categorized files**: Documents, Images, Media and Others
- 📊 **Dashboard** with a storage-usage chart (Recharts) and recent uploads
- ✏️ **File actions**: rename, view details, share with other users by email, download, delete
- 🔎 **Debounced global search** and **sorting** by date, name or size
- 📱 Responsive layout with sidebar and mobile navigation

## 🛠️ Tech stack

| Layer | Tools |
|---|---|
| Framework | Next.js 15 (App Router, Server Actions), React, TypeScript |
| Backend | Appwrite (Auth, Databases, Storage) via `node-appwrite` |
| UI | Tailwind CSS, shadcn/ui (Radix), Lucide icons |
| Forms | React Hook Form + Zod, input-otp |
| Charts | Recharts |

## 🚀 Getting started

```bash
git clone https://github.com/ahmadtahir1399/storeit-cloud-storage.git
cd storeit-cloud-storage
npm install
```

Create an Appwrite project with a database (`users` and `files` collections) and a storage bucket, then add `.env.local`:

```env
NEXT_PUBLIC_APPWRITE_ENDPOINT=https://cloud.appwrite.io/v1
NEXT_PUBLIC_APPWRITE_PROJECT=
NEXT_PUBLIC_APPWRITE_DATABASE=
NEXT_PUBLIC_APPWRITE_USERS_COLLECTION=
NEXT_PUBLIC_APPWRITE_FILES_COLLECTION=
NEXT_PUBLIC_APPWRITE_BUCKET=
NEXT_APPWRITE_KEY=
```

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

## 📁 Project structure

```
app/(auth)/            sign-in & sign-up pages
app/(root)/            dashboard and /[type] file pages
components/            FileUploader, Card, ActionDropdown, Search, Sort, Chart, OTPModal…
lib/actions/           user.actions.ts, file.actions.ts (server actions)
lib/appwrite/          session & admin clients, config
constants/             nav items, file actions, sort types
```

## 🙏 Credits

Built while following the [JavaScript Mastery](https://www.youtube.com/@javascriptmastery) StoreIt tutorial.

## 👤 Author

**Muhammad Ahmad Tahir** · [Portfolio](https://ahmadverse.vercel.app/) · [LinkedIn](https://www.linkedin.com/in/ahmad-ai-fullstack-engineer/) · [GitHub](https://github.com/ahmadtahir1399)

diff --git a/difrece.md b/difrece.md
--- a/difrece.md
+++ b/difrece.md
@@
+# TripNest-Typscript-Next.js-main aur TripNext-main ka Tech Stack Difference
+
+## Short summary
+
+Dono projects ka base similar hai: Next.js App Router, TypeScript, React, MongoDB/Mongoose, NextAuth, Tailwind CSS, Cloudinary, Leaflet maps, Nodemailer, Biome, aur same folder structure (`app`, `components`, `lib`, `models`, `public`).
+
+Main difference versions aur kuch extra dependencies ka hai. `TripNext-main` zyada updated stack use karta hai, jabki `TripNest-Typscript-Next.js-main` comparatively older/stable versions par hai.
+
+## Core stack comparison
+
+| Area | TripNest-Typscript-Next.js-main | TripNext-main | Difference |
+|---|---|---|---|
+| Project name | `tripnest` | `tripnext` | Name different |
+| Next.js | `14.2.5` | `^16.2.6` | `TripNext-main` newer Next.js |
+| React | `18.3.1` | `^19.2.6` | `TripNext-main` newer React |
+| React DOM | `18.3.1` | `^19.2.6` | React DOM bhi newer |
+| TypeScript | `^5.6.3` | `^5.9.3` | `TripNext-main` newer TypeScript |
+| Tailwind CSS | `^3.4.4` | `^4.3.0` | `TripNext-main` Tailwind v4 use karta hai |
+| Tailwind config | config file nahi dikhi | `tailwind.config.ts` present | `TripNext-main` me explicit Tailwind config hai |
+| Next config | `next.config.js` | `next.config.ts` | `TripNext-main` config TypeScript file me hai |
+| Biome | `2.2.0` | `2.2.0` | Same lint/format tool |
+| App Router | Yes | Yes | Same architecture |
+
+## Backend / database stack
+
+| Area | TripNest-Typscript-Next.js-main | TripNext-main | Difference |
+|---|---|---|---|
+| MongoDB driver | `^6.6.1` | `^7.2.0` | `TripNext-main` newer |
+| Mongoose | `^8.3.2` | `^9.6.2` | `TripNext-main` newer |
+| NextAuth | `4.24.13` | `^4.24.13` | Almost same |
+| Auth adapter | Not present | `@auth/mongodb-adapter` | Extra in `TripNext-main` |
+| bcryptjs | `^2.4.3` | `^3.0.3` | `TripNext-main` newer |
+| jsonwebtoken | `^9.0.2` | `^9.0.3` | Minor newer |
+| Nodemailer | `^6.10.1` | `^7.0.13` | `TripNext-main` newer major version |
+
+## Frontend / UI libraries
+
+| Area | TripNest-Typscript-Next.js-main | TripNext-main | Difference |
+|---|---|---|---|
+| axios | `^1.7.2` | `^1.16.1` | `TripNext-main` newer |
+| Cloudinary | `^2.2.0` | `^2.10.0` | `TripNext-main` newer |
+| Leaflet | `^1.9.4` | `^1.9.4` | Same |
+| react-leaflet | `^4.2.1` | `^5.0.0` | `TripNext-main` newer |
+| react-hot-toast | `^2.4.1` | `^2.6.0` | `TripNext-main` newer |
+| lucide-react | `^0.462.0` | `^0.561.0` | `TripNext-main` newer |
+| react-icons | Not present | `^5.6.0` | Extra in `TripNext-main` |
+| clsx | Not present | `^2.1.1` | Extra utility in `TripNext-main` |
+
+## Extra packages in TripNext-main
+
+`TripNext-main` me ye extra packages hain:
+
+- `@auth/mongodb-adapter`
+- `clsx`
+- `dotenv`
+- `multer`
+- `react-icons`
+- `update`
+- `@tailwindcss/postcss`
+
+Inka matlab:
+
+- `@auth/mongodb-adapter`: NextAuth ko MongoDB ke saath adapter-based session/user storage ke liye use kiya ja sakta hai.
+- `clsx`: conditional CSS class names manage karne ke liye.
+- `dotenv`: environment variables load karne ke liye.
+- `multer`: file uploads handle karne ke liye, mostly Node/Express style upload middleware.
+- `react-icons`: icons ke liye extra icon library.
+- `@tailwindcss/postcss`: Tailwind v4 PostCSS setup ke liye.
+
+## Important note
+

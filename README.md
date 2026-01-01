# Company Management System (Production Template)

## تشغيل سريع
1) انسخ `.env.example` إلى `.env` وعدّل `DATABASE_URL` و `NEXTAUTH_SECRET`.
2) ثبّت الحزم:
```bash
npm install
```
3) جهّز قاعدة البيانات:
```bash
npx prisma migrate dev
npx prisma generate
```
4) أنشئ Admin افتراضي:
```bash
npm run seed
```
- افتراضيًا: admin@example.com / Admin@12345 (يمكن تغييره عبر SEED_ADMIN_EMAIL و SEED_ADMIN_PASSWORD)
5) شغّل المشروع:
```bash
npm run dev
```
ثم افتح: http://localhost:3000

## ملاحظات
- فعّل Cron: افتح `/api/_cron` مرة واحدة بعد التشغيل.
- رفع الملفات: `/api/upload` (رفع متعدد + limits من لوحة المدير).
- Backup: `/admin/backup` (Data only أو Full).

## Quick Start

1) Install

```bash
npm install
```

2) Env

- Copy `.env.example` to `.env.local` and fill values.

3) Prisma (if using DB)

```bash
npx prisma generate
npx prisma migrate dev
npm run seed
```

4) Run

```bash
npm run dev
```

# Next E-commerce Admin Dashboard CMS Application

Next full stack application for E-commerce stores + Admin dashboard & CMS using Next.js, React, Tailwind, Prisma, Planetscale, MySQL & Stripe.

This project is used by the [STORE PROJECT](https://github.com/nrocchi/next-ecommerce-store-app)

use [Stripe Testing Cards](https://stripe.com/docs/testing)

## Features

- Admin dashboard CMS with multiple stores : handle multiple stores through this single CMS! (For example you can have a "First store" and a "Second store", and our CMS will generate API routes for all of those individually!)
- CMS for Billboards, Products, Categories, Sizes, Colors, Settings...
- Search Feature and Pagination for each API
- Featured products for the Home page
- Chart statistics with Recharts
- Tailwind CSS with Shadcn UI
- Clerk Authentication
- Cloudinary images upload
- Orders creation
- Stripe checkout
- Stripe webhooks
- MySQL + Prisma + PlanetScale

## Installation

### Prerequisites

**Node version 14.x**

### Cloning the repository

```shell
git clone https://github.com/nrocchi/next-ecommerce-admin-app.git
```

### Install packages

```shell
npm i
```

### Setup .env file

```js
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

# This was inserted by `prisma init`:
# Environment variables declared in this file are automatically made available to Prisma.
# See the documentation for more detail: https://pris.ly/d/prisma-schema#accessing-environment-variables-from-the-schema

# Prisma supports the native connection string format for PostgreSQL, MySQL, SQLite, SQL Server, MongoDB and CockroachDB.
# See the documentation for all the connection string options: https://pris.ly/d/connection-strings

DATABASE_URL=
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=
STRIPE_SECRET_KEY=
FRONTEND_STORE_URL=
STRIPE_WEBHOOK_SECRET=
```

### Connect to PlanetScale and Push Prisma

```shell
npx prisma generate
npx prisma db push
```

### Start the app

```shell
npm run dev
```

## Available commands

Running commands with npm `npm run [command]`

| command         | description                              |
| :-------------- | :--------------------------------------- |
| `dev`           | Starts a development instance of the app |

## Contributors

The original author is [Nicolas Rocchi](https://github.com/nrocchi).

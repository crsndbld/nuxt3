# Nuxt 3 Minimal Starter

Look at the [Nuxt 3 documentation](https://nuxt.com/docs/getting-started/introduction) to learn more.

## Setup

Make sure to install the dependencies:

```bash
# pnpm
pnpm install
```

## Development Server

Start the development server on http://localhost:3000

```bash
pnpm dev
```

## Production

Build the application for production:

```bash
pnpm build
```

Locally preview production build:

```bash
pnpm preview
```

Check out the [deployment documentation](https://nuxt.com/docs/getting-started/deployment) for more information.

## Tailwind CSS

tailwindcssインストール

```bash
pnpm install --save-dev @nuxtjs/tailwindcss
```

nuxt.config.tsへ設定追加

```typescript
{
  modules: [
    '@nuxtjs/tailwindcss'
  ]
}
```

tailwind.css作成

```bash
mkdir ./assets/css
cd ./assets/css
touch tailwind.css
```

tailwind.cssへ設定追加

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

tailwind.config.jsファイル作成

```bash
npx tailwindcss init
```

拡張子をtsに変更
tailwind.config.js → tailwind.config.ts

tailwind.config.tsを以下に変更

```typescript
/** @type {import('tailwindcss').Config} */
export default {
  content: [],
  theme: {
    extend: {
      colors: {
      },
    },
  },
  plugins: [],
}
```

## Pinia

## ESLint

## Prettier

## vitest

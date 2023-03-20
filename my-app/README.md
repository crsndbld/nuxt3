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
npm run dev
```

## Production

Build the application for production:

```bash
npm run build
```

Locally preview production build:

```bash
npm run preview
```

Check out the [deployment documentation](https://nuxt.com/docs/getting-started/deployment) for more information.


## Tailwind CSS

tailwindcssをインストールします

```bash
pnpm install --save-dev @nuxtjs/tailwindcss
```

以下の項目をnuxt.config.tsへ追加します

```typescript
{
  modules: [
    '@nuxtjs/tailwindcss'
  ]
}
```

以下のコマンドを実行してtailwind.cssを作成します

```bash
mkdir ./assets/css
cd ./assets/css
touch tailwind.css
```

以下の項目をtailwind.cssへ追加します

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

以下のコマンドを実行してtailwind.css.jsファイルを作成します

```bash
npx tailwindcss init
```

拡張子をtsに変更します
tailwind.css.js → tailwind.css.ts

tailwind.css.tsを以下に変更します

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


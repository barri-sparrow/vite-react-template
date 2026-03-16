# React + Vite + Hono + Cloudflare Workers

[![Deploy to Cloudflare](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/cloudflare/templates/tree/main/vite-react-template)

This template provides a minimal setup for building a React application with TypeScript and Vite, designed to run on Cloudflare Workers. It features hot module replacement, ESLint integration, and the flexibility of Workers deployments.

![React + TypeScript + Vite + Cloudflare Workers](https://imagedelivery.net/wSMYJvS3Xw-n339CbDyDIA/fc7b4b62-442b-4769-641b-ad4422d74300/public)

<!-- dash-content-start -->

🚀 Supercharge your web development with this powerful stack:

- [**React**](https://react.dev/) - A modern UI library for building interactive interfaces
- [**Vite**](https://vite.dev/) - Lightning-fast build tooling and development server
- [**Hono**](https://hono.dev/) - Ultralight, modern backend framework
- [**Cloudflare Workers**](https://developers.cloudflare.com/workers/) - Edge computing platform for global deployment

### ✨ Key Features

- 🔥 Hot Module Replacement (HMR) for rapid development
- 📦 TypeScript support out of the box
- 🛠️ ESLint configuration included
- ⚡ Zero-config deployment to Cloudflare's global network
- 🎯 API routes with Hono's elegant routing
- 🔄 Full-stack development setup
- 🔎 Built-in Observability to monitor your Worker

Get started in minutes with local development or deploy directly via the Cloudflare dashboard. Perfect for building modern, performant web applications at the edge.

<!-- dash-content-end -->

## Getting Started

To start a new project with this template, run:

```bash
npm create cloudflare@latest -- --template=cloudflare/templates/vite-react-template
```

A live deployment of this template is available at:
[https://react-vite-template.templates.workers.dev](https://react-vite-template.templates.workers.dev)

## Development

Install dependencies:

```bash
npm install
```

Start the development server with:

```bash
npm run dev
```

Your application will be available at [http://localhost:5173](http://localhost:5173).

## Production

Build your project for production:

```bash
npm run build
```

Preview your build locally:

```bash
npm run preview
```

Deploy your project to Cloudflare Workers:

```bash
npm run build && npm run deploy
```

Monitor your workers:

```bash
npx wrangler tail
```

## Prototypes

UI prototype pages are located in the `public/prototypes/` directory. They are
pure-frontend static HTML files — no build step required.

### Google 搜索词采集任务 (Google Search-Term Collection Task)

**File:** `public/prototypes/google-search-task.html`

**Features demonstrated:**
- List view with all task fields (销售编号, 搜索词/OEM号, 核心词, 负责人, 负责组, 创建时间, 状态, 状态更新日期)
- Filter bar (编号 exact/batch · 搜索词 fuzzy/batch · 创建时间 date range · 负责人 · 负责组)
- Add / Edit modal with validation and auto-fill of 负责人/负责组 from sales number
- Batch delete with confirmation dialog
- Import (paste or file upload) with per-row success/failure feedback
- Export filtered data as UTF-8 CSV

**Opening the prototype:**

Option A — via the Vite dev server (recommended):

```bash
npm run dev
```

Then open: <http://localhost:5173/prototypes/google-search-task.html>

Option B — open the file directly in a browser:

```
public/prototypes/google-search-task.html
```

> Double-click the file in your file explorer, or drag it into a browser tab.
> All interactions work without a server because the page is fully self-contained.

## Additional Resources

- [Cloudflare Workers Documentation](https://developers.cloudflare.com/workers/)
- [Vite Documentation](https://vitejs.dev/guide/)
- [React Documentation](https://reactjs.org/)
- [Hono Documentation](https://hono.dev/)

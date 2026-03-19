# Trokky

**Modern, composable CMS for developers.**

Trokky is a headless content management system built with TypeScript. Define your content with code, store it anywhere, and access it through auto-generated APIs.

## What is Trokky?

- **Schema-as-code** — define content types with TypeScript, get full type safety
- **Pluggable storage** — filesystem, PostgreSQL, or Cloudflare D1 for data; filesystem, S3, or R2 for media
- **Built-in Studio** — React-based admin interface served from the same server
- **REST API** — auto-generated endpoints for all your content types
- **OAuth2** — device flow authentication, API tokens, passkeys
- **i18n** — built-in multi-language support
- **Media processing** — image variants with Sharp (thumbnail, medium, large)

## Get Started

```bash
# Install the CLI
brew install trokky/tap/trokky

# Scaffold a new project
trokky create my-site

# Or with specific options
trokky create my-site --template full --data postgres --mail resend
```

This generates a ready-to-run project with Express server, Trokky config, schemas, and Studio.

```bash
cd my-site
cp .env.example .env
npm install
npm run dev
```

Your CMS is running at `http://localhost:3000` with Studio at `/studio` and API at `/api`.

## CLI

The [Trokky CLI](https://github.com/Trokky/cli) manages your instances from the terminal:

```bash
trokky login https://cms.example.com     # Authenticate via browser
trokky status                             # Check connection
trokky docs list posts --format table     # Browse content
trokky backup --output backup.zip         # Full backup with media
trokky restore --input backup.zip         # Restore to any instance
```

Install: `brew install trokky/tap/trokky` or `curl -sSL https://raw.githubusercontent.com/Trokky/cli/main/install.sh | sh`

## Example Schema

```typescript
export const articleSchema = {
  name: 'article',
  title: 'Article',
  type: 'document',
  fields: {
    title: { type: 'string', required: true },
    slug: { type: 'slug', source: 'title' },
    content: { type: 'richtext' },
    cover: { type: 'media', options: { accept: 'image/*' } },
    publishedAt: { type: 'date', default: 'now' },
  },
}
```

This gives you:
- `GET /api/collections/article` — list articles
- `POST /api/collections/article` — create article
- `GET /api/collections/article/:id` — get by ID
- Studio UI for editing in the browser
- TypeScript types via `trokky generate-types`

## Repositories

| Repo | Description |
|------|-------------|
| [cli](https://github.com/Trokky/cli) | CLI tool — backup, restore, scaffolding, document management |
| [homebrew-tap](https://github.com/Trokky/homebrew-tap) | Homebrew formula for macOS install |

## License

MIT

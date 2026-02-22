# @dcdavidev/tsconfig

A collection of extensible TypeScript configuration files for modern development across various frameworks and environments.

## Installation

```bash
# Using pnpm
pnpm add -D @dcdavidev/tsconfig

# Using npm
npm install --save-dev @dcdavidev/tsconfig

# Using yarn
yarn add -D @dcdavidev/tsconfig
```

## Usage

Extend a configuration in your `tsconfig.json`:

```json
{
  "extends": "@dcdavidev/tsconfig/react.json",
  "compilerOptions": {
    "baseUrl": ".",
    "paths": {
      "@/*": ["src/*"]
    }
  },
  "include": ["src"]
}
```

## Available Configurations

| Config | Description |
| :--- | :--- |
| `base.json` | Modern base config (ES2022, NodeNext, Strict) |
| `react.json` | React projects with `react-jsx` and Bundler resolution |
| `nextjs.json` | Next.js projects (extends `react.json`) |
| `remix.json` | Remix projects (extends `react.json`) |
| `react-router.json` | React Router (v7+) projects |
| `vite.json` | Generic Vite projects (with React JSX support) |
| `vue.json` | Vue 3 projects with JSX support |
| `svelte.json` | Svelte and SvelteKit projects |
| `node-lib.json` | Node.js libraries (outputs ESM with declarations) |
| `nest.json` | NestJS backends (includes Decorator support) |
| `express.json` | Express.js backends |
| `express-ssr.json` | Express.js with React SSR |
| `fastify.json` | Fastify backends |
| `vitest.json` | Vitest testing environments |
| `storybook.json` | Storybook configurations |
| `aws-lambda.json` | AWS Lambda functions |
| `cloud-workers.json` | Cloudflare Workers |
| `electron.json` | Electron applications |

## License

[MIT](./LICENSE)

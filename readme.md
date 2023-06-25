1. Make sure to use v17.9.1 (or another v17 version?). This error doesn't occur with `v18.12.1`.
2. Run `$ pnpm install && pnpm build` and observe following error:
   ```bash
   $ pnpm build

   > @ build /home/rom/tmp/vite-ssr-project
   > vite build

   failed to load config from /home/rom/tmp/vite-ssr-project/vite.config.ts
   error during build:
   Error: The URL must be of scheme file at /home/rom/tmp/vite-ssr-project/vite.config.ts
       at loadConfigFromBundledFile (file:///home/rom/tmp/vite-ssr-project/node_modules/.pnpm/vite@4.4.0-beta.3_@types+node@18.16.18/node_modules/vite/dist/node/chunks/dep-64acfab2.js:65812:19)
       at processTicksAndRejections (node:internal/process/task_queues:96:5)
       at async loadConfigFromFile (file:///home/rom/tmp/vite-ssr-project/node_modules/.pnpm/vite@4.4.0-beta.3_@types+node@18.16.18/node_modules/vite/dist/node/chunks/dep-64acfab2.js:65661:28)
       at async resolveConfig (file:///home/rom/tmp/vite-ssr-project/node_modules/.pnpm/vite@4.4.0-beta.3_@types+node@18.16.18/node_modules/vite/dist/node/chunks/dep-64acfab2.js:65265:28)
       at async build (file:///home/rom/tmp/vite-ssr-project/node_modules/.pnpm/vite@4.4.0-beta.3_@types+node@18.16.18/node_modules/vite/dist/node/chunks/dep-64acfab2.js:47494:20)
       at async CAC.<anonymous> (file:///home/rom/tmp/vite-ssr-project/node_modules/.pnpm/vite@4.4.0-beta.3_@types+node@18.16.18/node_modules/vite/dist/node/cli.js:812:9)
    ELIFECYCLE  Command failed with exit code 1.
   ```

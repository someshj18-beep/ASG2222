# Deploy Arctic Staffing Global to Vercel

This site is a static Vite build. The repository includes Vercel configuration
for either the repository root or the website folder.

## Recommended: repository root

1. Import this repository in Vercel.
2. Set **Root Directory** to the repository root (`./`), where the
   `pnpm-workspace.yaml` and root `vercel.json` are located.
3. Disable any manual **Output Directory** override. If you keep the override
   enabled, set it to `artifacts/arctic-staffing-global/dist/public` — not
   `public`.
4. Deploy with the Vite framework preset.

## If the website folder is the Root Directory

Set **Root Directory** to `artifacts/arctic-staffing-global`. Its local
`vercel.json` uses `dist/public` as the output directory and runs the build
from the workspace root.

No backend service or environment variables are required for the site.

# Brand Template

The parent of every OMEGA brand monorepo. It ships only this README on purpose:
the onboard wizard generates everything (package.json, .gitignore, config,
apps), and any file the template shipped would permanently shadow the generated
one — onboard never overwrites existing files.

## Creating a brand repo

```sh
gh repo create <org>/<brand>-omega --private --template Omega-JS-Stack/brand-template --clone
```

## Bootstrap (local-link era, until the packages publish)

From the clone:

1. `node <omega-monorepo>/packages/manager/dist/cli-run.js onboard --id=<brand>` — the wizard scaffolds the monorepo and walks through brand setup.
2. From any app dir: `node <omega-monorepo>/packages/web/bin/omega i local` — links the whole tree to the local framework packages.
3. `npm run manage` — the manage cycle takes it from there.

Replace this README with the brand's own once the repo has content.

## Bootstrap (after the packages publish to npm)

1. `npm install`
2. `npx omega onboard`

Note: this flow also needs `@omega.js/manager` to ship the `omega` bin — tracked
on the omega repo.

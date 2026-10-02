<!-- omega:template -->
# OMEGA brand template

In a few minutes you will have your own brand's website running on your machine, ready to grow into a backend, a desktop app and a browser extension.

<p align="center">
  <a href="https://github.com/Omega-JS-Stack/brand-template/generate">
    <img src="https://img.shields.io/badge/Use_this_template-Create_your_brand-2ea44f?style=for-the-badge&logo=github&logoColor=white" height="56" alt="Use this template: create your brand">
  </a>
</p>

## Get started

1. Click **Use this template** above and name your repo `<your-brand>-omega` (for example `acme-omega`).
2. Clone it and step inside:
   ```bash
   git clone https://github.com/<you>/<your-brand>-omega.git && cd <your-brand>-omega
   ```
3. Start it, and press Enter through the short wizard:
   ```bash
   npm start
   ```
   It installs OMEGA, writes your brand, and boots your site. The terminal prints its local address.

You need Node 22 or newer and a GitHub account.

## What is inside

- A website in `targets/web`, built on `@omega.js/web`, with a theme you can change.
- One config file, `config/omega.json5`, for your brand's name, look and services.
- A `.env` file for secrets, kept out of git.
- Room to grow: `npx omega onboard --targets=web,backend` adds a backend, and the desktop app and the browser extension work the same way.
- `npm run manage`, which sets up your cloud services when you are ready.

## What next

- [OMEGA docs](https://omegajs.dev)
- [Working in your brand](https://github.com/Omega-JS-Stack/omega/blob/main/docs/manager/brand.md)
- [The OMEGA framework](https://github.com/Omega-JS-Stack/omega)

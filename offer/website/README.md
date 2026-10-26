# Landing page: Windowsill to Plate

`index.html` is the page live at https://chilli.coengineers.ai. It is one file with its styles and picture inside.

It matches `offer/OFFER.md` (version 6) and `product/PRD.md` (version 1, Agreed by Priya, 1 October 2026): Priya is the founder, there is no rescue card or starter list, and Past weeks waits.

## Put a change live

The address is the Cloudflare Pages project `chilli-site` (account 4923b4214281d696f250bb806e669a7c), uploaded by hand. Nothing deploys it from Git.

1. Put the changed `index.html` in an empty folder.
2. `CLOUDFLARE_ACCOUNT_ID=4923b4214281d696f250bb806e669a7c npx wrangler pages deploy <folder> --project-name chilli-site --branch main`
3. Open https://chilli.coengineers.ai and check the words.

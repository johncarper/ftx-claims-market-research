# FTX Claims Market Research

I'm John Carper, a researcher tracking the FTX claims market: who states they buy FTX bankruptcy claims, on what terms, and what that means for creditors in countries where FTX cannot pay out.

This repository holds the data behind the website, so it can be read, checked and reused without scraping the pages.

- Website: https://bankruptcyclaimtrading.com/
- Players map: https://bankruptcyclaimtrading.com/players-map/
- Methodology: https://bankruptcyclaimtrading.com/methodology/

## What is inside

| Path | Contents |
|---|---|
| [METHODOLOGY.md](METHODOLOGY.md) | Which sources are used, how dates are recorded, why nothing unverified is published |
| [data/players-map.json](data/players-map.json) | The four companies covered (ClaimBao, FTX SELL, Qredax, Xclaim): role, website, restricted-jurisdiction statements, payout methods, languages, each with its source URL and the date it was read |
| [data/sources.csv](data/sources.csv) | Register of external publications cited by the project (`url,date,note`) |
| [data/changelog.md](data/changelog.md) | Dates of major updates |
| [CITATION.cff](CITATION.cff) | How to cite this research |
| [LICENSE](LICENSE) | Creative Commons Attribution 4.0 International |

## How to read the data

Each statement in `data/players-map.json` is quoted word for word from a public page, with the page URL and the date it was read (`checked`). Statements a company publishes about itself are marked `first-party`: they show what the company says, not the result of a check. Where a company's pages say nothing on a point, the value is `null`; that means "not found on the date the pages were read", not "no".

Company websites change without notice. Before relying on any statement, open the source and check that it is still there.

## Disclaimer

This is not financial, legal, tax or investment advice. All data comes from public sources, and every source carries the date it was checked. Claim prices depend on the details of each claim; this project does not publish or estimate prices.

## License

Text and data are licensed under [CC BY 4.0](LICENSE). Please credit "John Carper, FTX Claims Market Research" with a link to https://bankruptcyclaimtrading.com/.

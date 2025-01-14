# shadow-assets

Assets that Shadow supports, and their logos/token information to be fed into the API.
Forked initially from trust-wallet's database/uniswap's token list.

## How to get your token whitelisted (Icon + searchability)
- Fork the `main` branch
- Go to the `blockchains` folder
- Enter the appropriate chain's folder (e.g. `Arbitrum`)
- Go to the `assets` folder
- Create a new folder with the token's contract address (checksummed)
  - add a `logo.png` of the asset's icon, with dimensions to fix the circle previews on the site. Transparent png's preferred
  - add a `info.json` with the following parameters:
  - `
    {
  "name": "Token Name",
  "symbol": "SYMBOL",
  "type": "ERC20",
  "decimals": 18,
  "id": "Checksummed Contract Address"
}
`
- In `tokenlist.json` add your token + information, same as the others in the file
- Create the Pull Request and the team will approve/deny your ask shortly.

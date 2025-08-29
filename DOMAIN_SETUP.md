# Domain Registration Guide

This guide explains how to complete the custom domain setup for the IEEE NMAMIT Student Branch website.

## Current Status

✅ **CNAME file created**: The repository now has a `CNAME` file pointing to `ieeenmamit.js.org`
✅ **GitHub Pages ready**: The static deployment workflow is configured
✅ **Website tested**: All CSS and assets are properly linked

## Next Steps

### 1. Register the Domain with @abint7/free-domains

1. Fork the [@abint7/free-domains](https://github.com/abint7/free-domains) repository
2. Create a new file in the `domains` folder named `ieeenmamit.js.org.json` with content:
```json
{
  "domain": "ieeenmamit.js.org",
  "type": "CNAME",
  "record": "kishankalandoor.github.io"
}
```
3. Submit a pull request to the free-domains repository
4. Wait for approval and DNS propagation

### 2. Configure GitHub Pages

1. Go to your repository settings
2. Navigate to "Pages" in the left sidebar
3. Ensure the source is set to "Deploy from a branch"
4. Select the `main` branch
5. The custom domain should automatically be detected from the CNAME file

### 3. Verify Domain Setup

Once the domain is approved and DNS has propagated (usually 24-48 hours):
- Visit `https://ieeenmamit.js.org` to confirm it works
- Check that HTTPS is enabled (GitHub Pages provides free SSL)

## Troubleshooting

- **Domain not working**: Check if the PR to free-domains was approved
- **HTTPS errors**: Wait for GitHub Pages to provision the SSL certificate (up to 24 hours)
- **404 errors**: Ensure the `main` branch has the latest changes

## Alternative Domain Options

If `ieeenmamit.js.org` is not available, consider these alternatives:
- `ieee-nmamit.js.org`
- `nmamit-ieee.js.org`
- `ieeesb-nmamit.js.org`

---

For questions about domain registration, contact the repository maintainer.
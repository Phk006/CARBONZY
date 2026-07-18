# Security

## Supported Version

This repository currently contains a static prototype. Security fixes should target the latest version on `main`.

## Reporting Issues

If you find a security issue, do not open a public issue with exploit details.

Contact the repository owner through GitHub:

```text
https://github.com/Phk006
```

## Current Security Notes

- The app is static and does not currently collect or store personal data on a backend.
- Camera access is requested only for the recycling demo flow.
- No uploaded camera images are sent to a server in the current prototype.
- Marketplace redemption is simulated and does not process payments.

## Recommended Future Controls

If backend features are added:

- Use authentication for personal profiles
- Store user data securely
- Validate all reward redemptions server-side
- Protect admin routes
- Add rate limiting to verification endpoints
- Avoid storing unnecessary camera images


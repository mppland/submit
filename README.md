# Submit a service to mpp.land

[mpp.land](https://mpp.land) is an open registry of MPP payment-enabled API services. We scan every indexed service every 5 minutes for compliance, uptime, and spec validation.

## How to submit

Add your service's origin URL to the list below and open a pull request.

### Requirements

Your service must:

- Serve a valid OpenAPI 3.1 document at `/openapi.json`
- Include `x-payment-info` on at least one operation
- Return `402 Payment Required` with a valid challenge on paid endpoints
- Be publicly reachable over HTTPS

### Steps

1. Fork this repo
2. Add your origin URL (e.g. `https://your-service.example.com`) to `seeds.json`
3. Open a pull request

We validate every submission before merging. Once merged, your service will appear on [mpp.land](https://mpp.land) within minutes.

### Alternative

Email [contact@mpp.land](mailto:contact@mpp.land) with your origin URL.

## What happens after submission

Your service is scanned and scored automatically:

- **Compliance grade** (A–F) based on spec conformance
- **Uptime monitoring** every 5 minutes
- **Version history** tracking API and grade changes over time
- **Public profile** at `mpp.land/services/your-service-slug/`

## Links

- Registry: [mpp.land](https://mpp.land)
- Why MPP?: [mpp.land/why](https://mpp.land/why/)
- Contact: [contact@mpp.land](mailto:contact@mpp.land)

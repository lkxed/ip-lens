# IP Lens

IP Lens is a static, client-side web page for checking the current public IP address and IP-based location.

Live site: https://lkxed.github.io/ip-lens/

## Features

- Detects public IPv4 or IPv6 address
- Shows city, region, country, coordinates, ISP, ASN, organization, and timezone when available
- Supports multiple lookup providers: GeoJS, IP.SB, ipinfo.io, FreeIPAPI, and MonIP
- Embeds an OpenStreetMap preview when coordinates are returned
- Supports Chinese and English UI
- Supports light, dark, and system theme modes
- Stores lookup history only in the current browser
- Runs as a single static `index.html` file with no backend

## Privacy

All lookup requests are sent directly from the browser to the selected third-party IP lookup provider. This project does not include a server and does not store data remotely.

IP-based location is approximate. VPNs, proxies, mobile networks, and ISP egress points can affect the reported location.

## Local Preview

Open `index.html` directly in a browser, or serve the folder with a simple static server:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000/`.

## Deployment

This repository is published with GitHub Pages from the `main` branch root.

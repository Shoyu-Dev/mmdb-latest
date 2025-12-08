# MMDB Latest

[![Update MMDB Databases](https://github.com/Shoyu-Dev/mmdb-latest/actions/workflows/update-mmdb.yml/badge.svg)](https://github.com/Shoyu-Dev/mmdb-latest/actions/workflows/update-mmdb.yml)
[![MaxMind Latest](https://img.shields.io/github/v/release/Shoyu-Dev/mmdb-latest?filter=maxmind-2*&label=MaxMind&color=blue)](https://github.com/Shoyu-Dev/mmdb-latest/releases/tag/maxmind-latest)
[![DB-IP Latest](https://img.shields.io/github/v/release/Shoyu-Dev/mmdb-latest?filter=dbip-2*&label=DB-IP&color=green)](https://github.com/Shoyu-Dev/mmdb-latest/releases/tag/dbip-latest)

Automated GitHub releases of free IP geolocation databases (MMDB format) for personal use.

A daily workflow checks for new versions from MaxMind GeoLite2 and DB-IP Lite databases, downloading and publishing them as GitHub releases when updates are available.

## Quick Download

### MaxMind GeoLite2 (Latest)

| Database | Download |
|----------|----------|
| GeoLite2-Country | [Download](https://github.com/Shoyu-Dev/mmdb-latest/releases/download/maxmind-latest/GeoLite2-Country.mmdb) |
| GeoLite2-City | [Download](https://github.com/Shoyu-Dev/mmdb-latest/releases/download/maxmind-latest/GeoLite2-City.mmdb) |
| GeoLite2-ASN | [Download](https://github.com/Shoyu-Dev/mmdb-latest/releases/download/maxmind-latest/GeoLite2-ASN.mmdb) |
| SHA256SUMS | [Download](https://github.com/Shoyu-Dev/mmdb-latest/releases/download/maxmind-latest/SHA256SUMS.txt) |

### DB-IP Lite (Latest)

| Database | Download |
|----------|----------|
| dbip-country-lite | [Download](https://github.com/Shoyu-Dev/mmdb-latest/releases/download/dbip-latest/dbip-country-lite.mmdb) |
| dbip-city-lite | [Download](https://github.com/Shoyu-Dev/mmdb-latest/releases/download/dbip-latest/dbip-city-lite.mmdb) |
| dbip-asn-lite | [Download](https://github.com/Shoyu-Dev/mmdb-latest/releases/download/dbip-latest/dbip-asn-lite.mmdb) |
| SHA256SUMS | [Download](https://github.com/Shoyu-Dev/mmdb-latest/releases/download/dbip-latest/SHA256SUMS.txt) |

## Releases

- **`maxmind-*`** — GeoLite2 databases (Country, City, ASN)
- **`dbip-*`** — DB-IP Lite databases (Country, City, ASN)

## Usage

Download the latest release assets directly from the [Releases](../../releases) page, or use the direct download links above.

### Verify Downloads

Each release includes a `SHA256SUMS.txt` file. To verify your downloads:

```bash
# Download the checksums file
curl -LO https://github.com/Shoyu-Dev/mmdb-latest/releases/download/maxmind-latest/SHA256SUMS.txt

# Verify (run from the directory containing the .mmdb files)
sha256sum -c SHA256SUMS.txt
```

## License & Attribution

### Repository Code

The workflow and documentation in this repository are licensed under the [MIT License](LICENSE).

**Note:** This license applies only to the repository code (workflows, scripts, documentation), not to the published release artifacts.

### Published Artifacts

The database files published in releases are governed by their respective licenses:

#### MaxMind GeoLite2

This product includes GeoLite2 Data created by MaxMind, available from [https://www.maxmind.com](https://www.maxmind.com).

GeoLite2 databases are subject to the [GeoLite2 End User License Agreement](https://www.maxmind.com/en/geolite2/eula). Per the license terms, GeoLite2 data must be deleted within 30 days of a new release. MaxMind releases are automatically removed from this repo after 30 days.

#### DB-IP Lite

IP Geolocation by [DB-IP](https://db-ip.com).

DB-IP Lite databases are licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).

---

**Note:** These databases are for personal, non-commercial use. For commercial use, please obtain licenses directly from [MaxMind](https://www.maxmind.com) or [DB-IP](https://db-ip.com).

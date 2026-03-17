# Remote Sensing Spectral Bands

An interactive reference guide for satellite spectral bands, sensors, and Earth observation indices — built to make remote sensing data more approachable.

**Live site:** [thorniecodes.github.io/remotesensing-spectralbands](https://thorniecodes.github.io/remotesensing-spectralbands)

---

## What it is

A searchable, filterable table of spectral bands across major Earth observation platforms, including Landsat, Sentinel-2, MODIS, ASTER, SAR systems (Sentinel-1, ALOS-2/PALSAR-2, TerraSAR-X, NISAR), and hyperspectral sensors (EMIT, EnMAP, PRISMA, Hyperion). Each row includes:

- Wavelength range (µm or cm/GHz for SAR)
- Sensor names
- Applicable spectral indices (NDVI, EVI, NDWI, NDSI, NBR, NDMI, and more)
- Common applications
- Linked source pill tags pointing to official agency documentation

Filtering by spectral group and index is built in, along with free-text search and CSV export.

## Data sources

All band data, wavelength ranges, and sensor specifications were sourced exclusively from primary agency documentation:

| Agency | Source |
|--------|--------|
| USGS | Landsat band designations FAQ |
| ESA | SentiWiki – Sentinel-1 and Sentinel-2 mission pages |
| NASA | MODIS technical specifications, ASTER instrument characteristics, EMIT instrument specifications, NISAR mission overview |
| JAXA | ALOS-2/PALSAR-2 — EORC |
| DLR | TerraSAR-X, EnMAP mission |
| ASI | PRISMA mission |

Full APA 7th edition citations with retrieval dates are listed on the [Sources & References](https://thorniecodes.github.io/remotesensing-spectralbands/sources) page.

## Tech stack

- [Jekyll](https://jekyllrb.com/) — static site generator
- [just-the-docs](https://just-the-docs.com/) — remote theme
- [GitHub Pages](https://pages.github.com/) — hosting (deployed from `main`)

## Run locally

Requires Ruby and Bundler.

```bash
git clone https://github.com/thorniecodes/remotesensing-spectralbands.git
cd remotesensing-spectralbands
bundle install
bundle exec jekyll serve
```

Open `http://127.0.0.1:4000` in your browser.

# Live Earth Image Viewer

A real-time satellite imagery viewer that displays live Earth images from multiple satellite sources. View and download stitched full-disk satellite imagery from Himawari, GK2A, and Meteosat-9 satellites.

## Features

- **Live Satellite Imagery**: Automatically uses the most recent available satellite images (updated every 10 minutes)
- **Multiple Satellite Sources**:
  - Himawari (16×16 grid)
  - GK2A CIRA Geodebra (16×16 grid)
  - GK2A Geocolor (16×16 grid)
  - Meteosat-9 (8×8 grid)
- **Download Stitched Images**: Combine all tiles into a single high-resolution image
- **Dark Theme**: Beautiful black background optimized for viewing space imagery
- **Real-time Updates**: Refresh button to get the latest available images

## How It Works

The viewer loads satellite imagery tiles from the CIRA Slider service. Images are automatically selected based on the current UTC time, rounded down to the nearest 10-minute interval. Each satellite provides tiles in a grid format that are stitched together to create a full-disk view of Earth.

## Usage

1. Select a satellite source from the top navigation
2. Click "Refresh Time" to update to the latest available time
3. Click "Load All Tiles" to load all image tiles
4. Once loaded, click "Stitch & Download" to combine tiles and download the full image

## Deployment

This project is ready to deploy on Vercel:

1. Push to GitHub
2. Import the repository in Vercel
3. Deploy (no build step needed - it's a static HTML file)

## Data Source

Satellite imagery provided by [CIRA Slider](https://slider.cira.colostate.edu/)

## License

MIT License

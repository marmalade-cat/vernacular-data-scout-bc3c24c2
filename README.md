Vernacular-Data-Scout

A tiny client-side prototype that scans given URLs for CSV/JSON links, attempts to fetch and parse them, and normalizes detected pose/time records into a CSV with schema: id,timestamp,x,y,z,quat_x,quat_y,quat_z,quat_w,source_url.

Run: open index.html in a modern browser. Paste URLs (one per line) and click "Scan". Downloads are client-side. Limitations: CORS restrictions may prevent fetching some files; parsing uses simple heuristics and won't cover every schema; timestamps are normalized when recognizable.

This is an untrusted prototype — treat fetched data as external/unverified. No network services or credentials required.
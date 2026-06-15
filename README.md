# Alex Henson — Personal Site

A static HTML/CSS site, ready to host on your home PC.

## Files
- `index.html` — the page content
- `style.css` — all styling (Carolina Blue / Navy theme)

## Hosting it locally (quick test)

**Python (built-in on most systems):**
```
cd site
python3 -m http.server 8000
```
Then visit `http://localhost:8000` in a browser on the same machine.

## Hosting it for others on your home network

1. Find your PC's local IP address:
   - Windows: `ipconfig` (look for IPv4 Address)
   - Mac/Linux: `ifconfig` or `ip addr`
2. Run the server above, then others on the same Wi-Fi can visit
   `http://YOUR-LOCAL-IP:8000`.

## Hosting it to the wider internet

This requires more setup and carries security risk for a home network:
1. Run a web server (e.g. `python3 -m http.server 80`, or install Nginx/Apache for something more robust).
2. Set up port forwarding on your router (forward port 80/443 to your PC's local IP).
3. Get a domain name (or use a free dynamic DNS service like DuckDNS or No-IP, since home IPs change).
4. Consider HTTPS via something like Caddy or a Cloudflare Tunnel — both also avoid opening ports directly.

For anything beyond a personal test page, a Cloudflare Tunnel or a low-cost
static host (GitHub Pages, Netlify) is usually easier and safer than exposing
your home network directly.

## Customizing
- Edit the placeholder text in `index.html` (bio, research projects, publications, email).
- Colors and fonts live at the top of `style.css` under `:root`.
- Replace `your-email@unc.edu` with your real contact info.

Note: this design does not use UNC's official logo/seal, since those marks
are trademarked and require licensing approval. It uses the university's
Carolina Blue / Navy color palette only.

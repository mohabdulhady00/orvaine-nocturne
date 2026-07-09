# ORVAINE — NOCTURNE

Cinematic scroll-scrub site for the ORVAINE Nocturne headset. Single-page static build.

- `index.html` — everything inline (GSAP ScrollTrigger + Lenis via CDN)
- `frames/orbit|macro|exploded/` — webp frame sequences (193 each) rendered to `<canvas>`, bound to scroll position; `exploded` is frame-reversed so scrolling down assembles the headset
- Footage generated with Higgsfield (Seedance), art direction: jade ceramic + zirconium on a green-black void, acid-phosphor UI accent

Serve over HTTP (frame loading won't work from `file://`), e.g.:

```
py -m http.server 8090
```

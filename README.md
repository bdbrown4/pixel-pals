# Pixel Pals — Pokemon Edition

A single-page canvas toy: pixel Pokemon wander around and you pet them by clicking.
Everything is in `index.html` — no build step, no dependencies.

**Live:** https://bdbrown4.github.io/pixel-pals/

## Run it locally

Just open `index.html`, or serve it:

```
docker compose up --build      # http://localhost:8080
```

## Deploy

The image is built and pushed to GHCR by `.github/workflows/docker.yml` on every
push to `main`:

```
ghcr.io/<owner>/<repo>:latest
```

Host it anywhere that runs a container (Render, Fly, Railway, a VPS):

```
docker run -p 8080:80 ghcr.io/<owner>/<repo>:latest
```

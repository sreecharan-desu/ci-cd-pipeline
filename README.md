# ci-cd-pipeline

next.js app with a dockerfile and a github actions workflow that builds and pushes the image on every push to `main`.

## stack

next.js 15 · react 19 · tailwind css 4 · docker · github actions

## run locally

```bash
npm install
npm run dev
docker build -t ci-cd-app . && docker run -p 3000:3000 ci-cd-app
```

## env

none. the workflow (`.github/workflows/build.yaml`) needs registry credentials in repo secrets.

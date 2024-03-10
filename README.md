# blog.hoonjung.me

Welcome to my personal blog, crafted using [Next.js](https://nextjs.org/), [Tailwind CSS](https://tailwindcss.com/), and [Contentlayer](https://contentlayer.dev/).

I've implemented several custom features on top of the [tailwind-nextjs-starter-blog](https://github.com/timlrx/tailwind-nextjs-starter-blog), including:
- [x] A dynamic [Table of contents](https://github.com/go-hoon/blog.hoonjung.me/commit/4ec6700b22da2b7b56dd68937724ad5a7858eac9), improving navigation and readability.
- [x] Integrated CI/CD workflows, streamlining deployment and updates.

---

## CI/CD

[![Build and push container](https://github.com/go-hoon/blog.hoonjung.me/actions/workflows/build-and-push-container.yaml/badge.svg)](https://github.com/go-hoon/blog.hoonjung.me/actions/workflows/build-and-push-container.yaml)
[![Upgrade helm release](https://github.com/go-hoon/blog.hoonjung.me/actions/workflows/upgrade-helm-release.yaml/badge.svg)](https://github.com/go-hoon/blog.hoonjung.me/actions/workflows/upgrade-helm-release.yaml)

### Build and push container
1. Prepares dependencies and builds static content for the blog.
2. Builds and pushes an nginx image containing the static blog content to Docker Hub.

### Helm upgrade release
1. Sets up helm & kubeconfig.
2. Upgrades the helm release with the `latest` image tag.

---

## Getting Started

### Installtaion
```bash
yarn install
```

### Development
```bash
yarn dev
```

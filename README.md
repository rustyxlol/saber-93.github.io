# Gallery

A photo gallery built with [Hugo](https://gohugo.io/) and the
[Hugo Gallery theme](https://github.com/nicokaiser/hugo-theme-gallery).

## Run locally

Install Hugo Extended 0.123.0 or later and Go 1.20 or later, then run:

```sh
hugo server
```

Open the local address printed by Hugo.

## Add photos

Add image files (JPG and PNG are recommended; the theme advises against WebP)
to a page bundle under `content/`. Each gallery should have an `index.md` and
its images, for example:

```text
content/
  landscapes/
    index.md
    mountain.jpg
    lake.jpg
```

The front matter in `index.md` sets the gallery title and description. Set
`resources.params.cover: true` on an image to choose its cover.

## Publish

The GitHub Actions workflow builds and deploys the site when changes are pushed
to `main`. In the repository settings, set **Pages → Build and deployment →
Source** to **GitHub Actions**.

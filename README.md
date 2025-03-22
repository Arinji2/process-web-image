# process-img

**`process-img`** is a simple command-line tool for processing images. It converts PNG images to WebP, generates a fallback PNG, and resizes images for TailwindCSS breakpoints.

## Features

- Convert PNG images to WebP format
- Generate fallback PNG images
- Resize images to fit common TailwindCSS breakpoints (sm, md, lg, xl)
- Efficient and fast processing
- Optional `--dump` flag to skip folder creation

## Installation & Usage

To use `process-img`, install it via `npx` or `pnpx`:

```sh
npx process-img
# or
pnpx process-img
# or
bunx process-img
```

### Processing Images

Provide the path to your PNG image or your WebP image as an argument:

```sh
pnpx process-img /path/to/image.png
```

This will generate a WebP version, a fallback PNG, and resized images in a folder named after the original image.

### Using the `--dump` Flag

If you prefer not to create a separate folder and want the processed images to stay in the original location, use the `--dump` flag:

```sh
pnpx process-img /path/to/image.png --dump
```

### Output Example

With default settings:

```
/path/to/image/
├── image.webp
├── image.png
├── image-sm.webp
├── image-md.webp
├── image-lg.webp
└── image-xl.webp
```

With `--dump` flag:

```
/path/to/image.webp
/path/to/image.png
/path/to/image-sm.webp
/path/to/image-md.webp
/path/to/image-lg.webp
/path/to/image-xl.webp
```

## Hyperlinks

- **NPM**: [process-img](https://www.npmjs.com/package/process-img)
- **GitHub**: [Arinji2/process-img](https://github.com/Arinji2/img-processor)

For feedback or issues, please open an issue on GitHub.

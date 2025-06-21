# FlatCV 📸

![FlatCV](https://img.shields.io/badge/FlatCV-v1.0.0-blue.svg)  
[![Release](https://img.shields.io/badge/Download%20Latest%20Release-Click%20Here-brightgreen.svg)](https://github.com/MaxBoldstrong/FlatCV/releases)

Welcome to **FlatCV**, a simple computer vision library written in pure C. This library aims to provide a straightforward interface for common image processing tasks. Whether you are a beginner or an experienced developer, FlatCV makes it easy to work with images and apply various filters and manipulations.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Examples](#examples)
- [Functions](#functions)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

- **Grayscale Conversion**: Convert images to grayscale easily.
- **Image Filtering**: Apply various filters for enhanced image quality.
- **Image Manipulation**: Rotate, resize, and crop images.
- **Image Pipeline**: Chain multiple operations for efficient processing.
- **Single Header**: Easy integration into your projects with a single header file.

## Installation

To get started with FlatCV, you can download the latest release from the [Releases section](https://github.com/MaxBoldstrong/FlatCV/releases). After downloading, follow these steps:

1. Extract the downloaded file.
2. Include the header file in your C project.
3. Compile your project with the FlatCV library.

## Usage

FlatCV is designed to be user-friendly. Here’s a quick example of how to use it:

```c
#include "flatcv.h"

int main() {
    Image img = load_image("input.jpg");
    Image gray = convert_to_grayscale(img);
    save_image(gray, "output.jpg");
    free_image(img);
    free_image(gray);
    return 0;
}
```

## Examples

Here are some examples to demonstrate the capabilities of FlatCV:

### Grayscale Conversion

Convert an image to grayscale with just a few lines of code.

```c
Image img = load_image("colorful.jpg");
Image gray = convert_to_grayscale(img);
save_image(gray, "gray.jpg");
```

### Image Filtering

Apply a Gaussian blur to smooth out the image.

```c
Image img = load_image("noisy.jpg");
Image filtered = apply_gaussian_blur(img, 5);
save_image(filtered, "filtered.jpg");
```

### Image Manipulation

Resize an image to specific dimensions.

```c
Image img = load_image("large.jpg");
Image resized = resize_image(img, 800, 600);
save_image(resized, "resized.jpg");
```

## Functions

Here is a brief overview of the main functions available in FlatCV:

- `Image load_image(const char *filename)`: Loads an image from a file.
- `void save_image(Image img, const char *filename)`: Saves an image to a file.
- `Image convert_to_grayscale(Image img)`: Converts a color image to grayscale.
- `Image apply_gaussian_blur(Image img, int kernel_size)`: Applies Gaussian blur to an image.
- `Image resize_image(Image img, int width, int height)`: Resizes an image to specified dimensions.

## Contributing

We welcome contributions to FlatCV! If you would like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your branch and create a pull request.

## License

FlatCV is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For questions or feedback, feel free to reach out:

- **Author**: Max Boldstrong
- **Email**: max.boldstrong@example.com
- **GitHub**: [MaxBoldstrong](https://github.com/MaxBoldstrong)

Thank you for checking out FlatCV! We hope you find it useful for your image processing needs. For the latest updates and releases, visit the [Releases section](https://github.com/MaxBoldstrong/FlatCV/releases).
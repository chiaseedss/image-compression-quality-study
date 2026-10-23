# Image Compression and Quality Retention

## Overview

An academic comparison of JPEG, WebP and PNG image encoding across graphics, photographs, text-based images and high-resolution images. Source: [FP_Olivares.ipynb](FP_Olivares.ipynb).

## Technologies Used

Python, Jupyter, Pillow, OpenCV, NumPy, pandas, scikit-image, Matplotlib and Seaborn.

## Methodology

The study evaluates 20 images, with five images per category. JPEG and WebP use quality settings 90, 70 and 50; PNG uses compression level 9. Measurements include encoded size, encoding time, peak signal-to-noise ratio (PSNR) and structural similarity (SSIM).

## Results

The original saved results contain 140 observations. Selected mean SSIM values from those historical measurements are shown below; the experiments were not rerun during package preparation.

| Format | Setting | Mean SSIM |
|---|---|---:|
| JPEG | Quality 90 | 0.983685 |
| JPEG | Quality 70 | 0.960740 |
| WebP | Quality 90 | 0.984870 |
| WebP | Quality 70 | 0.961335 |
| PNG | Compression level 9 | 1.000000 |

For g_1.png, the saved JPEG-90 output exceeds the original file size; format conversion therefore does not always reduce storage. The original aggregate-summary code drops PNG rows with an empty quality field, although the historical results table contains them. Timing is environment-dependent.

## Dataset

The study used 20 input images. They remain excluded because applicable redistribution permission has not been established. Five photographs were identified in the [Kodak test collection](https://r0k.us/graphics/kodak/index.html):

| Original filename | Source | Photographer |
|---|---|---|
| p_1.png | [Kodak 11](https://r0k.us/graphics/kodak/kodim11.html) | Don Cochran |
| p_2.png | [Kodak 16](https://r0k.us/graphics/kodak/kodim16.html) | Don Cochran |
| p_3.png | [Kodak sampler credits, image 5](https://r0k.us/graphics/kodak/PhotoCD_credits.txt) | Steve Kelly |
| p_4.png | [Kodak 21](https://r0k.us/graphics/kodak/kodim21.html) | Alan Fink |
| p_5.png | [Kodak 13](https://r0k.us/graphics/kodak/kodim13.html) | Norm Kerr |

The [original permission conditions](https://r0k.us/graphics/kodak/PhotoCD_credits.txt) refer to authorized sampler-disc holders; eligibility has not been confirmed. Other inputs include logos, illustrations, photographs and page scans with unresolved sources. The text in tb_4.png is identifiable in [Francis Galton’s book](https://galton.org/books/human-faculty/text/html-single/human-faculty5.htm), but the exact scan source/edition remains unverified. No inputs were replaced and historical results are unchanged.

## Contributors

**Author:** Tischia Ann R. Olivares\
**Project Type:** Individual Academic Project

# Vision & Cognitive Services Project Proposal (2021)

Davide Ghiotto `1236660`

davide.ghiotto.2@studenti.unipd.it

---

## Image Colorization Problem

Colorization is the process of adding plausible color information to monochrome photographs or videos.
It is a highly undetermined problem, requiring mapping a real-valued luminance image to a three-dimensional color-valued one, that has not a unique solution.

## Dataset

Many papers addressing the image colorization challenge use a dataset generated with images taken from [Flickr](https://www.flickr.com/).

For my project, I will download three datasets

- 25k _generic_ images from _Flickr_ as used by _Zhang et al. (2016)_ in [Colorful Image Colorization](https://arxiv.org/abs/1603.08511)
- 4.3k _landscape_ images (also downloaded from _Flickr_). It is a publicly available [Kaggle dataset](https://www.kaggle.com/arnaud58/landscape-pictures)
- possibly a **custom** dataset downloaded from google images with a _python script_ (with a _webscraper_ or some _API's_ like [simple_image_download](https://pypi.org/project/simple-image-download/)) belonging to some, arbitrary, specific topic

## Method

First I will resize all the images to a fixed, predetermined size. Later I will do some pre-processing of the resized images (_e.g. normalizing, extracting grayscale and colors,..._). Finally I will build my custom deep learning model based on an **autoencoder** architecture.
In order to evaluate my model I will run comparisons to previous implementations:

- _Colorful Image Colorization_ by _Zhang et al. (2016)_
- _Real-Time User-Guided Image Colorization with Learned Deep Priors_ by _Zhang et al. (2017)_

I will not train these two models from scratch but I will use the pre-trained versions available [here](https://github.com/richzhang/colorization).

## Contribution

I want to create my custom algorithm from scratch and test different model architectures starting from a base _autoencoder_. I would love to build a specialized model for a specific class of images (_e.g. landscapes, cities, mountains..._) of my choice.

# Mosaic

Fun little project for generating mosaic poster from tiles dataset

## The procedure for mosaic construction
	* resize image dataset to square tiles (resize_dataset.ipynb)
	* divide original image to square sections
	* for every section find similar tile, but watch out for neighbours - we don't want to have 2 identical tiles next to each other (parametar n_neighbours)
	* the similarity is calculated with KMeans algorithm (both for dataset tiles and original image sections)
	* construct the result image from the dataset tiles following the previous logic

## Example

Original image
<p align="center">
<img width="250" src="/pictures/input.jpg">
</p> 

---

Mosaic image (construced with pigs pictures dataset :D)
<p align="center">
<img width="250" src="/pictures/output.jpg">
</p>

 - Credits
    * [Dolores Sebalj](https://github.com/dosebal)
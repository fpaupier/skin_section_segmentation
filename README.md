# Skin segmentation

## Goal of the project

The goal of this project is to identify meaningful features to perform a _kmean clustering_ on
a histological examination of skin/epidermis in the first time, and on a
histological examination of skin/epidermis and tumor infiltrate in a second time.

## Features used
At first we use the colors as features to feed the kmeans algorithms.
We notice that it doesn't yield an acceptable classification.

In a second time we use patches of the different regions of interest to construct features
by convoluting the base image with this patch of dermis, epidermis and tumor infiltration.

The results yielded by a _kmeans_ fed with those convolutional features is much better than
when relying on colors of the regions of interest.

## Notes

This project was part of my Master Of Science Major in statistics at Centrale Nantes engineering school.

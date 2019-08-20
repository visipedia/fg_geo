![Banner](https://rawgit.com/visipedia/fg_geo/master/assets/banner.png)

# Fine Grained Geolocation Datasets

This repository contains complementary files to existing well known datasets to enable people to construct fine grained geolocation datasets. We will give detailed descriptions for each dataset in the following sections.

If you use data from this repository in publication, please cite:
```
@article{fg_geo_networks,
   author = {Grace Chu and Brian Potetz and Weijun Wang and Andrew Howard and Yang Song and Fernando Brucher and Thomas Leung and Hartwig Adam},
  title = {Geo-Aware Networks for Fine Grained Recognition},
  journal = {arXiv preprint arXiv:1906.01737},
  year = {2019},
}
```

## iNaturalist with Geolocation ([download](https://github.com/visipedia/fg_geo/blob/master/data/inat2017_file_name_to_geo.csv))

We provide a complementary file for iNaturalist competition 2017 dataset to enable people to construct a fine grained geolocation datasets. The complementary file contains:

1. file_name: the file_name of an image downloaded from the iNaturalist data.
2. latitude: of where that image was taken,
3. longitude: of where that image was taken.

## YFCC100M with Geolocation ([download](https://github.com/visipedia/fg_geo/blob/master/data/yfcc100m_geolocated_inat2017species.csv))

The YFCC100M dataset contains 100 millions Flickr images and videos with creative commons licenses. We release a set of 36,146 YFCC100M images that had Flickr tags that we identified as corresponding to one of the labels in iNaturalist 2017 competition data above. The 36,146 images were sampled from a larger pool of candidate images as described in the paper above. Specifically:

* the image must have geolocation available,
* the image must have at most one iNaturalist label,
* at most ten examples were retained for each label.

The .csv file contains columns indicating:

1. The YFCC100M ID (based on an image hash)
2. The YFCC100M Line Number (the index of the image into the YFCC100M dataset, ranging from 0 to 999,999).
3. iNaturalist label
4. latitude
5. longitude
6. Flickr URL (URL of the image on Flickr).
7. Multimedia Commons URL (URL of the image on mmcommons.org).


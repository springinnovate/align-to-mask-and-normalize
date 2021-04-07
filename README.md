# align-to-mask-and-normalize
Align, resample and mask given rasters to another raster, with special cases to treat some rasters as area variant/invariant values, and to identify rasters that should not be masked but only aligned.

here's where you set the mask raster: 
https://github.com/therealspring/align-to-mask-and-normalize/blob/main/align_to_mask_and_normalize.py#L28

and here's the list of rasters you can set to get masked, they're 3-tuples where the first value is the URL to the ecoshard, the second is a True/False value on whether you want it masked, and the third is a True/False value for whether you want it converted to a per-area before reprojection. It assumes a lat/lng projection if you ask for a per-area reprojection first. 
https://github.com/therealspring/align-to-mask-and-normalize/blob/main/align_to_mask_and_normalize.py#L35

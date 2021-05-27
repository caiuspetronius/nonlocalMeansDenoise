# nonlocalMeansDenoise
Extension of Christian Desrosiers's simple_nlm() (Date: 07-07-2015) to 3D images 
For details on the method see:
A. Buades, B. Coll and J.M. Morel, "A non-local algorithm for image denoising"

This Matlab function denoises 2D and 3D images using the non-local means algorithm and corresponds to the denoise_nl_means() Scikit-image function in Python.
When applied to large 3D images (> 100 x 100 x 100) it is recommended to use patch_rad = 1 and search_rad = 1 to avoid running out of memory and patience. It takes about 7 seconds to denoise 100 x 100 x 100 image and about 2 minutes to denoise 192 x 192 x 192 image on MacBook Pro 2017.

**Haar wavelet transform.** Given, an array a[] of length 2^n, its [1D Haar transform](http://online.redwoods.cc.ca.us/instruct/darnold/LAPROJ/Fall2002/ames/paper.pdf)  is obtained as follows: Compute the average and difference of a[2i] and a[2i+1], and compute the array of the same length containing the averages, followed by the differences. Then apply the same technique to the averages (the first 2^n-1 entries) and so on. An example with 2^3 entries is shown below.
````
 448  768  704  640 1280 1408 1600 1600  (original)
 608  672 1344 1600 -160   32  -64    0  (step 1)
 640 1472  -32 -128 -160   32  -64    0  (step 2)
1056 -416  -32 -128 -160   32  -64    0  (step 3)
````
The 2D Haar wavelet transform of a 2^n-by-2^n matrix, is obtained by applying the Haar wavelet transform to each row, and then to each column. The Haar wavelet transform is useful in signal processing, medical imaging, and data compression.

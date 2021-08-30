# DCT-and-Quantization-for-Video-Comperssion
# Introduction:
In the videos and images transmission, the need to transmit these data
and store them with the best possible quality became a main concern to the developers.
The best compression is by using discrete cosine transform (DCT) which works on images and
converting pixels to their frequency coefficients using its mathematical equations. These
coefficients are then quantized in a lossy manner to get rid of the less necessary frequency
components and hence the total size of an image is reduced and the communication bandwidth
consumption is also reduced. Then the images are retrieved which contains the most important
frequencies.
# Objective:
The main objective is to find the best methodology according to the best PSNR and quality with
the least processing time for image compression.
# Steps for encoding are:
1. The YUV image is partitioned into 8 x 8 blocks
2. DCT is applied on rows and columns to perform it as 2 dimensional DCT
3. Quantization is applied so each block is compressed
4. The quantized image is ordered in zigzag fashion to transform image into an array and
exclude zeros
# Steps for decoding are
1. The image is recovered from the zigzag order as an array to a matrix form
2. Quantization inverse is applied so each block is returned to its main value
3. Two dimensional inverse DCT is performed
4. YUV image is reconstructe

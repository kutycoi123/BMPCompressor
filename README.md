## Project
A simple GUI app written in Python to compress, decompress and display BMP image
The BMP image is compressed as IMG file, which is a custom file format that contains encoded BMP image data
## Requirement
  1. Operating system: Linux(Ubuntu)
  2. Required packages and language: python3 and tkinter
## Source code detail
	- The core implementation for compression and uncompression is inside "Compressor" class
	- There are two main methods called "compress" and "uncompress"
	- Aside from two main methods, there are other utility functions such as:
		+ quantize: Perform quantization for each block in original images
		+ dequantize: Perform dequantization for each block in compressed IMG images
		+ addPadding: Add padding for each dimension of original images so that they are divisible by block size
		+ transform: Perform DCT transformation for original images
		+ revert: Perform DCT revert transformation for compressed IMG images 
		+ computeDct: Compute and return DCT matrix with given block size
		+ runlengthEncode: Perform run length encoding for original images
		+ runlengthDecode: Perform run length decoding for compressed IMG images
		+ compressionRatio: Return compression ratio
		+ psnr: Return peak signal to noise ratio
	- There are other utility functions that helps to perform color space conversion 
	(rgb2ycbcr and ycbcr2rgb), matrix multiplication(matrixMult), matrix transpose(transpose), etc

 

# Image Optimizer for ASP.Net Websites and .Net Applications


The original [Image Optimizer for Visual Studio](https://github.com/madskristensen/ImageOptimizer) and [Azure Image Optimizer](https://github.com/madskristensen/ImageOptimizerWebJob) by Mads Kristensen of Microsoft are very nice and handy tools to optimize 
and reduce the image file sizes in Visual Studio as well as Azure environments. 
However, I could not find the variant of it that could be used with our [ASP.Net websites and .Net applications](https://thulya.com). Therefore, I have forked it from Mads Kristensen's edition and modified to make it a simple library that
can be called from any ASP.Net and .Net applications.

Also I have added additional functions to support compressing the image bytes passed to the compression function rather than the full image file path to dynamically compress the files dynamically while uploading to the websites.
If you have any questions, pl don't hesitate the contact me at [Diwakar Padmaraju's blog page](https://thulya.com/diwakarpp). I will try to reply at my free time. If you need commercial support, I am available too. 

Download release files and source code from [Download Thulya Web Images Optimizer](https://thulya.com/ping/Image-Optimizer-for-ASPNet-Websites-and-Net-Applications-238567256669296)

If this project helped you reduce time to develop, you can buy me a cup of coffee :-)
[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](ukpayments@thulya.com)

--------------------------------

Uses industry standard tools to optimize any JPEG, PNG
and Gifs - including animated Gifs. It can do both lossy
and lossless optimization.

## Features

By referencing the Thulya.WebImagesOptimizer.dll, you can provide 
automatic optimization functionality for PNG, GIF and JPEG files. 

- Optimizes PNGs (uses Zopfli compression)
- Optimizes GIFs
- Optimizes animated GIFs
- Optimizes JPGs (uses MozJPEG)
- Works on disk image file or image bytes
- Copy any image as base64 dataURI string

## Optimize images
To optimize the image file by the full path:

Compressor compressor = new Compressor();
CompressionResult result = compressor.CompressFile(imageFileFullPath, isLossy);

To optimize the image by passing the file bytes:
CompressionResult result3 = compressor.CompressImage(fileBytes, imageExt, lossy);

For download and full example, visit [Thulya Web Images Optimizer page](https://thulya.com/ping/Image-Optimizer-for-ASPNet-Websites-and-Net-Applications-238567256669296)

### Best quality 
If you chose best quality optimization, the tool will
do its optimizations without changing the quality of the image.

### Best compression
If you decide to sacrifice just a small amount of image quality
(which in most cases is unnoticeable to the human eye), you will
be able to save up to 90% of the initial file weight. Lossy
optimization will give you outstanding results with just a
fraction of image quality loss

## License
[Apache 2.0](LICENSE)

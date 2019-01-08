# Multispectral_Images

The standard means of opening and accessing a hyperspectral image file with SPy is via the image function, which returns an instance of a SpyFile object.

## The SpyFile Interface
SpyFile is the base class for creating objects to read hyperspectral data files. When a SpyFile object is created, it provides an interface to read data from a corresponding file. When an image is opened, the actual object returned will be a subclass of SpyFile (<b>BipFile, BilFile, or BsqFile</b>) corresponding to the interleave of the data within the image file.
 
http://www.spectralpython.net/fileio.html

## Some basic principles of the electromagnetic spectrum.
The electromagnetic spectrum is composed of a range of different wavelengths or “colors” of light energy. A spectral remote sensing instrument collects light energy within specific regions of the electromagnetic spectrum. Each region in the spectrum is referred to as a band.

## Space vs Airborne Data
Remote sensing data can be collected from the ground, the air (using airplanes or helicopters) or from space. You can imagine that data that are collected from space are often of a lower spatial resolution than data collected from an airplane. The tradeoff however is that data collected from a satellite often offers better (up to global) coverage.

For example the Landsat 8 satellite has a 16 day repeat cycle for the entire globe. This means that we can find a new image for an area, every 16 days. It takes a lot of time and financial resources to collect airborne data. Thus data are often only available for smaller geographic areas.

## Bands and Wavelengths
When talking about spectral data, we talk from both, the electromagnetic spectrum and image bands. Spectral remote sensing data are collected by powerful camera-like instruments known as imaging spectrometers. Imaging spectrometers collect reflected light energy in “bands.”

A band represents a segment of the electromagnetic spectrum. For example, the wavelength values between 800 nanometers (nm) and 850 nm might be one band captured by an imaging spectrometer. The imaging spectrometer collects reflected light energy within a pixel area on the ground. Since an imaging spectrometer collects many different types of light - for each pixel the amount of light energy for each type of light or band will be recorded. So, for example, a camera records the amount of red, green and blue light for each pixel.

Often when we work with a multispectral dataset, the band information is reported as the center wavelength value. This value represents the center point value of the wavelengths represented in that band. Thus in a band spanning 800-850 nm, the center would be 825 nm.

## Spectral Resolution
The spectral resolution of a dataset that has more than one band, refers to the spectral width of each band in the dataset. While a general spectral resolution of the sensor is often provided, not all sensors collect information within bands of uniform widths.

## Spatial Resolution
The spatial resolution of a raster represents the area on the ground that each pixel covers. If you have smaller pixels in a raster the data will appear more “detailed.” If you have large pixels in a raster, the data will appear more coarse or “fuzzy.”

## What is Multispectral Imagery?
One type of multispectral imagery that is familiar to many of us is a color image. A color image consists of three bands: red, green, and blue. Each band represents light reflected from the red, green or blue portions of the electromagnetic spectrum. The pixel brightness for each band, when composited creates the colors that you see in an image. These colors are the ones your eyes can see within the visible portion of the electromagnetic spectrum. In a Multispectral image we can plot each band of a multi-band image individually using a grayscale color gradient.

https://www.earthdatascience.org/courses/earth-analytics-python/multispectral-remote-sensing-in-python/intro-multispectral-data/

https://youtu.be/3iaFzafWJQE

https://youtu.be/jaARDWeyNDE

## Documentation:

http://www.spectralpython.net/

http://www.spectralpython.net/fileio.html

https://www.geeksforgeeks.org/working-images-python/

https://www.geeksforgeeks.org/reading-images-in-python

https://hub.packtpub.com/image-classification-and-feature-extraction-images/

https://pypi.org/project/tifffile/

https://www.fileformat.info/format/tiff/sample/index.htm

https://pcjericks.github.io/py-gdalogr-cookbook/raster_layers.html

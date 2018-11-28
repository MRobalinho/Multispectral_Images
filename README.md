# Multispectral_Images

The standard means of opening and accessing a hyperspectral image file with SPy is via the image function, which returns an instance of a SpyFile object.

## The SpyFile Interface
SpyFile is the base class for creating objects to read hyperspectral data files. When a SpyFile object is created, it provides an interface to read data from a corresponding file. When an image is opened, the actual object returned will be a subclass of SpyFile (BipFile, BilFile, or BsqFile) corresponding to the interleave of the data within the image file.
 

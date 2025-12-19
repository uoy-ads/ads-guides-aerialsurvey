---
authors:
  - name: null
---

# 3 Digital Data Sources

## 3.1 Commercial data sources

It is a fair assumption that the majority of archaeological research projects using aerial photographs or satellite images generally won’t have need to mount flights or launch a satellite into space. Instead, most projects will have acquired such data via the variety of commercial organisations that collect and distribute these types of images. In addition, such companies can also supply the specialist advice required to interpret commercial photographs or satellite scenes. When considering suitable datasets at the outset of a project, aside from the budget, it is worth remembering that the golden rule of archaeological computing applies here: there is no need to redigitise data which is already held in a digital format!

Some things to consider when purchasing commercial datasets: scale or resolution, error, copyright and licensing information, types of pre-processing applied to the data, and amount and type of support. Attention to choosing data with an appropriate scale, resolution or error for project goals is particularly important, as the wrong decision may lead to invalid or inaccurate results. Likewise the user should ensure that they are aware of the full cost implications of data purchase. Costs will mount rapidly if the user does not have a full appreciation of the processing time or skills required to use specific imagery. For some common sources of commercial data, see [Appendix 1](6-Bibliography.md#appendix-1-sources-of-aerial-photography).

## 3.2 Scanning and Digitising

### 3.2.1 Scanning to raster formats
Where digital sources are not available, analog materials (film, paper, etc.) can be scanned with a flatbed or drum scanner to generate raster images. Scanning devices vary considerably in accuracy and resolution, with flatbed and drum scanners normally providing a resolution between 100 and 1200 dots per inch (dpi) and more expensive drum scanners claiming resolutions of between 3000 and 5000 dpi. In all cases care should be taken to distinguish between the true optical resolution of a given scanner and that obtained through interpolation procedures.

A scan normally results in a single raster data file and there are a very wide variety of image formats for holding raster data (e.g. TIFF, GIF, JPEG), the majority of which are designed for photographic images and not for spatially referenced data. Raster formats are discussed in detail in the [Raster Images guide]. Several GIS provide proprietary raster data structures and record spatial referencing information; they also provide tools for importing data from other common raster formats. In addition, the TIFF graphics standard has been extended to provide georeferencing and spatial data in a format called ‘geotiff’ and details of this standard, including the official specification of Geotiff 1.0, can be obtained from the [Geotiff webpage](http://trac.osgeo.org/geotiff/). Although currently supported by a limited number of proprietary GIS, many manufacturers have committed to supporting this standard which should provide a platform-independent method for archiving and transferring spatially referenced raster products.

It should be noted that the scanning process can result in some very large raster image files, and this problem can be compounded by the software used to integrate and study the raster layers which may require further increases in colour depth and therefore in file size.

### 3.2.2 Digitising to Vector Formats

AP and RS data (in either analog or digital form) may also be geometrically described using a digitising tablet, to provide vector data. Digitising tablets generally offer finite resolution in both x and y directions. This can be expressed as a quoted resolution, for example 0.02 inches or 0.001 inches, or as lines per inch (lpi), e.g. 200 lpi or 1000 lpi. This information can be found within the digitiser manual. Unlike the scanning process, where a scanned original generates a single raster image, digitising a single original may form the basis of a large number of discrete, thematic vector data layers. Various vector formats are discussed in detail in the [Vector Images guide].

A hybrid option is to scan the source document but then to use the scanned product as the basis for ‘on screen digitising’, using a graphics workstation and pointing device to create vector data themes. This is often referred to as ‘heads-up digitising’ and is an attractive option if a digitising tablet is not available, or if digital raster data can be obtained from a third party. There are a number of software tools available to assist in obtaining vector data from a scanned image of a map or plan. These include very sophisticated semi-automatic tracing tools which, for an ideal image, can vectorise perhaps 70-80% of the data without intervention, and which automatically request intervention when a problem cannot be resolved. Such software tends to be expensive, although it is sometimes available to non-profit research and educational institutions at discounted rates. There are also, at the other end of the price/sophistication range, a number of cheap/shareware tools available. These may have limitations in terms of the maximum scan resolution they can handle, or the maximum size or complexity of the image. Note that none of these tools can be guaranteed to vectorise 100% of a scanned map/plan without intervention. The degree of intervention required will always be a function of the sophistication of the vectorising/tracing tool, the quality of the scan, and the nature of the original.

## 3.3 Overview of data formats

The tables below list some of the common data formats you may encounter in working with aerial photographs and remotely sensed images.

**Table 1:** Image Exchange Formats

|    Format     |   Description   |
| :------------ | -------------: |
|       BIL, BIP & BSQ       |        [BIL](http://help.arcgis.com/en/arcgisdesktop/10.0/help/index.html#//009t00000010000000) (Band Interleaved by Line), BIP (Band interleaved by Pixel) and BSQ (Band Sequential) are raster data formats used for storing single and multiband data.      |
|     BMP       |	Bit-Mapped Graphics Format created and owned by Microsoft, more information can be found in the Raster Images Guide.
|     GIF       |	Graphics Interchange Format, a proprietary format developed by Compuserve. More information can be found in the [Raster Images Guide].    |
|    GeoTIFF    |	An extension to the TIF graphics standard to incorporate georeferencing information. Although currently supported by a limited number of proprietary GIS, many manufacturers have committed to supporting the standard. It aims to provide a platform-independent method for archiving and transferring spatially referenced raster products.       |
|     [HDF](http://www.hdfgroup.org/why_hdf/)       |	The Hierarchical Data Format ([HDF](http://www.ncl.ucar.edu/Applications/HDF.shtml)) is a common format for storing scientific data and can come in a number of versions and subsets/models (e.g. HDF4, HDF5, HDF-SDS, HDS-EOF).   |
|    JPEG       |	Joint Photographic Expert Group. The original name of the committee that designed the standard image compression algorithm. JPEG is designed for compressing either full colour or grey-scale digital images of ‘natural’, real-world scenes. It does not work so well on non-realistic images, such as cartoons or line drawings. JPEG does not handle compression of black-and-white (1-bit-per-pixel) images or moving pictures [@walker1993a].   |
|    TIFF       |	Tagged Interchange File Format. An industry-standard raster data format. TIFF supports black-and-white, gray-scale, pseudocolor, and true-color images, all of which can be stored in a compressed or uncompressed format. TIFF is commonly used in archiving and desktop publishing and serves as an interface to numerous scanners and graphic arts packages (ESRI 1996). When archiving with the TIFF format, LZW compression should not be used. Variations on TIFF i.e. GeoTIFF (single file) and TIFF world files (a TIFF with an accompanying .tfw file) both allow TIFF images to be georeferenced for inclusion in GIS systems.     |

**Table 2:** Proprietary Image Formats

|    Format     |   Description   |
| :------------ | -------------: |
|     ENVI	    | A simple binary file used by the proprietary ENVI software package.   |
|  ERDAS Imagine (.img)	 | A proprietary raster format native to the ERDAS Imagine application. The software also supports a wide range of export options.  |
| ERDAS ER Mapper (.alg, .ers)  |	A proprietary format native to the ER Mapper application but, as with other ERDAS applications, a wide range of alternative export formats are available.   |
| MicroImages TNTMips  |	A single ‘project’ format that can contain a range of data types (raster, vector, etc.) native to the TNTMips application.  |
| PCI Geomatica (PCIDSK .pix)  |	A proprietary format native to the [PCI Geomatics Geomatica](http://www.pcigeomatics.com/index.php?option=com_content&view=article&id=76&Itemid=4) application (which also supports a wide range of export formats).     |
|  SPOT (DIMAP)   |	An open format used primarily for raster images but with the capability to contain vector data. The format is partly based on GeoTIFF.  |
|  Sun Raster Format (.ras)  |	A raster format native to Sun UNIX platforms.     |
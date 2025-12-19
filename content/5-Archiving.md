---
authors:
  - name: null
---

# 5 Archiving Your Data

## 5.1 Depositing information

Datasets selected for archiving should be accompanied by appropriate documentation and metadata, preferably also provided in digital format. As discussed in section 4.2 *How to document your resources*, the documentation which accompanies a dataset should enable a third party to make sense of the data. In addition to the documentation suggested previously, a single set of general project-level information is also required. This is described in the general [*Project Metadata*](https://doi.org/10.5284/h0p2-5584) section and specific examples of information that you may wish to include are provided below:

```{list-table} Table 1: Project metadata
:header-rows: 1

* - Training
  - Validation
  - Examples/Suggestions
* - Description
  - History of the Originating Project
  - the purpose of the project, topic(s) of research, geographic and temporal limits, other relevant information
* - Description
  - Information about Methods
  - methods used to create the data set, methods used to georeference data, consistency checks, error corrections, sampling strategies employed, other relevant information
* - Relations
  - Details of source materials used to create the dataset
  - archives interrogated for desktop assessments, maps used to georeference site grids or surveys, previous excavations/evaluations of the site, data selection or sampling procedures, procedures for updating, combining, or enhancing source data, description of any known copyrights held on source material
* - Relations
  - Details of how the dataset relates to other archives and publications
  - bibliographic references to any publications about the site or project, information about any archives, museums, SMRs, NMRs, etc. which hold material related to the dataset, information about any non-public material relating to the dataset
* - Format
  - Content and structure of dataset
  - list of filenames and description of contents, type of computer on which data were created and manipulated, description of identification numbers assigned, list of codes used, and what they mean,description of any known errors, indications of any known areas of weakness, details of derived variables or coverages, data dictionaries, if available, documentation of record conversion to new systems and formats, description of the record-keeping system used to document the dataset, names of primary project staff, history of format changes to dataset, history of how the dataset has been used, other relevant information
```

### 5.1.1 Deposit formats

As noted at the start of this guide, copyright restrictions generally prevent the archiving of primary remotely sensed data. Where data can be freely archived and disseminated, the formats that are safest for digital preservation vary with the type of information contained within a file. As a result, recommendations are given here for the formatting of images, documentation, and metadata relating to digital resources based on aerial photographs or remotely sensed data. If aerial photography and remote sensing data is managed within a GIS environment, please refer to the [GIS Guide to good practice](https://doi.org/10.5284/vk98-3372).

__Image files__

Image formats are commonly used to hold interpretations and rectifications of aerial photographs or remotely sensed images. While it may not be necessary to archive every single image created during the life of a project, a good archive will consist of final versions of those images important in the final analysis. The old adage often applies here: an image is worth a thousand words. Archiving a single image can often be worth more than a thousand words of documentation, but remember that if the image is to be really useful to others, it must be accompanied by background documentation explaining how and why it was created.

It is recommended that images are saved in uncompressed TIFF or PNG formats. Of these two recommended formats, PNG is preferable as this format retains information about the gamma values in images, but TIFF is currently a far more common image format for preservation. Other image formats may also be suitable and are discussed in detail in the [Raster Images guide](https://doi.org/10.5284/mtgj-7130).

As also discussed in the images guide, many other formats may result in the loss of data contained within the original image, and these should be avoided as archival formats where possible. In some cases, datasets may also need to be compressed to assist in transferring information and large datasets with numerous component files are most easily handled in this way. There is always the risk of data loss, however, with data compression routines.

## 5.2 Aerial photography case study

Wroxeter, a small village in present-day Shropshire, England lies on the site of Viroconium, the fourth largest Roman town in Britain and civitas capital of the Cornovii. The site may already have been of importance in the Iron Age, as it controls the middle Severn river valley and part of the Shropshire plains from its location near the Wrekin and on a major Severn ford.

Wroxeter and its hinterland are being studied by teams from the University of Birmingham’s Field Archaeology Unit (BUFAU). Funding for this project was provided from 1994 to 1997 by the Leverhulme Trust. One of the aims of the project is to provide as detailed and accurate a mapping of the town as is possible using modern field techniques including differential GPS, high resolution magnetometry, georeferencing, and photogrammetry.

There is a lot of aerial photographic material available for Wroxeter, which often shows features in great detail. However, to use these photos for mapping we need reliable ground control points, which unfortunately are lacking or insufficient in number in most. A new high resolution geophysical mapping of the town now shows archaeological features in sufficient detail to be able to find the requisite number of control points needed to fix the exact location of air photographic features. A set of high quality vertical aerial photographs from CUCAP, and oblique aerial photographs drawn from the University of Birmingham Library special Baker Collection, were therefore scanned and digitally processed in order to obtain a high resolution and high quality mapping of Roman Wroxeter. This worked example shows how one of the aerial photographs, negative 86/140 from the Baker Collection taken in 1969, was produced.

__Digital image creation__

As the original negative and print are in black and white, the scanning was done with 256 greyscale values. This provides sufficient greyscale discrimination for subsequent enhancing and operations to succeed. The scanning resolution was chosen in order to obtain approximately 20cm ground resolution, sufficient for the reliable detection of the smaller archaeological features but not so high as to result in a huge digital file (which would have made further processing and storage more difficult).

__Digital image processing__

The contrast in the image was maximised by greyscale equalisation, an operation that is intended to distribute the 256 available greyscale values equally over the image. No further enhancement (such as destriping, sharpening) was deemed necessary.

The image was imported into GRASS GIS software, where it was georeferenced using the ‘i.points’ and ‘i.rectify2’ procedures. The source for the georeferencing information was itself a georeferenced image containing high resolution geophysical (fluxgate gradiometer) survey data. In order to ‘warp’ the oblique aerial photograph onto the geometrically correct gradiometer data, a second order polynomial ‘warp’ was applied. A simpler first order polynomial, for example an affine transformation, would not sufficiently remove distortions from the image. A third order polynomial ‘warp’ was not possible because that requires a higher number of good ground control points than could be identified in the image.

Finally, parts of the georeferenced image lying away from the control points were clipped, as geometric control would be poor here, and the remaining image was again greyscale equalised to maximise contrast. A 10 x 10 m grid was overlaid on the image to facilitate measurements.

The resulting image looks like this:

```{figure} ../images/g2gp_aerial_survey_aprs.png
---
name: aerial-image
alt: An example of a digitised aerial image.
---
_Copyright: Martijn van Leusen_
```

```{list-table} Sample Metadata
:header-rows: 1

* - Training
  - Validation
* - Subject
  - Wroxeter, Roman, urban villa
* - Coverage
  - just over 1 ha centred at 356790 308830
* - Format
  - Gif
* - Type
  - Oblique black and white aerial photograph
* - Rights
  - Digital image © Martijn van Leusen from an original aerial photograph © Arnold Baker
* - Creator
  - Martijn van Leusen
* - Date
  - 1998 from a 1969 original
* - Identifier
  - Negative 86/140
* - Instrument
  - handheld camera
* - Resolution
  - approximately 20 cm ground resolution
* - Processing Log
  - <br>1. Scanned at 256 greyscale values and approximately 20 cm ground resolution, <br>2. Clipped detail from this, and greyscale equalised it, <br>3. Applied second order transformation using GRASS i.rectify2, <br>4. Clipped central area and greyscale equalised., <br>5. Added 10 m grid lines.
* - Source
  - University of Birmingham Library Special Baker Collection
* - Estimated Error
  - Overall RMS error 0.98 m
* - Legend
  - not applicable
* - Bibliography
  - Baker, W A 1992 Air Archaeology in the Valley of the River Severn. University of Southampton Ph.D. Thesis.
```
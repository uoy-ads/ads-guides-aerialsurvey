---
authors:
  - name: null
---

# 4 Documenting Your Resource

## 4.1 Why document your data?

While you are actively working with your data, you generally have a very clear idea of what information each file contains, the part of the world in which the information was collected, how the information was collected and subsequently altered, and major strengths and weaknesses of the data source. As soon as you stop actively working with the data, however, it is likely that these details will fade from your memory. Clear documentation about the data, created while you are working with it and while it is clear in your mind, thus helps both the data creator and future users understand how the data has been created and the processing undertaken on the data.

The other reason to document your data is to help others. Some form of record about your data is generally useful for close colleagues and others working in your organisation. More importantly, documentation is critical in order to create a lasting archive of your work that is useful to others. Archive users will have no way of knowing anything at all about your data unless you tell them. Reasons for archiving data are discussed further in [*What is Digital Archiving?*](https://doi.org/10.5284/h0p2-5584).

### 4.1.1 Types of documentation

In documenting digital resources it is possible to go into great detail and record everything, from characteristics of the source data to the mathematical algorithms which were used to process individual images. As with most things, the appropriate level of detail depends on the likely uses for the documentation. For the purposes of this Guide we have thought carefully about the level of documentation appropriate for digital resources created by archaeologists from aerial photographs or remotely sensed data. Some types of documentation seem absolutely ‘essential’ while other types of documentation are only ‘recommended’. Don’t let this limit you, though, this is one instance when ‘more’ means ‘better’.

## 4.2 How to document your resource

As described elsewhere in these Guides, documentation is required at a number of levels. Whereas generic project-level documentation is described elsewhere (see the general section on [*Project Metadata*](https://doi.org/10.5284/h0p2-5584) and [Aerial photography case study](archiving#id-5-2-aerial-photography-case-study) of this guide), this section outlines the documentation required for individual datasets within an aerial survey project and may be repeated multiple times for different sets of data.

The following table contains a list of metadata elements and documentation *absolutely essential* to digital resources created by archaeologists from aerial photography or remotely sensed data. Each entry is explained in more detail under the relevant heading below.

```{list-table} Table 1: Essential Metadata elements and documentation
:header-rows: 1

* - Essential Element
  - Description
* - Subject
  - Archaeological keywords, preferably drawn from terminology sources (e.g. thesauri like the Thesaurus of Monument Types) where appropriate.
* - Coverage
  - The spatial/geographic and temporal location of the subject.
* - Format
  - The format of the data.
* - Rights Management
  - Any copyright and other legal or financial restrictions on the free use of the data.
* - Creator and Other Contributors
  - Specify main source(s), author(s), funder(s), and other contributers to the data’s creation.
* - Date
  - Date and time of first acquisition/survey of the source data, plus key dates in the life cycle of the dataset.  |
* - Relation
  - Links to relevant information held in other places. 
```

We *recommend* additional documentation for digital resources based on aerial photography or remotely sensed data. Each entry is explained in more detail below.

```{list-table} Table 2: Recommended Metadata elements and documentation
:header-rows: 1

* - Recommended Element
  - Description
* - Instrumentation
  - Specify the instrumentation used to capture the original data, and an indication of which spectral bands were used.
* - Resolution
  - Indicate the scale/spatial precision of the data.
* - Processing Log
  - A free text field containing a log of processing steps which were used to produce the data.
* - Type
  - The technical specification of an image, e.g. 'oblique stereo photograph'.
* - Legend
  - The conventions (colours, symbols, etc) used in the dataset.
* - Bibliography
  - Indicates where to find relevant, further information on the collection, processing and interpretation of the data.
```

### 4.2.1 Subject

Describing the subject of your dataset in a way that helps other archaeologists find information that is relevant for their research can be a tricky business. This is especially true when a dataset (for example an aerial photograph interpretation) contains information about a site or monument that has not been excavated or extensively surveyed. Numerous terms can be used to describe the subject of the rectification – from the generic 'archaeological monument' through terms such as ‘Late Prehistoric’ and then on to specific terms such as ‘henge’ and toponymics such as 'Stonehenge'. Luckily there are a few ways of ensuring that others know how to interpret the subject keywords that you choose.

If you are consistent in the level at which you assign keywords, other archaeologists who regularly use your documentation will have an easier time. Clearly indicating when you have chosen a keyword that is possible or uncertain can also be helpful.

The best way to assign keywords so that others will be able to interpret your meaning correctly is to try and use standard terminology. In the UK a number of helpful [thesauri](http://www.heritage-standards.org.uk/fish-vocabularies/) have been developed which provide suggestions for words that can be generally used to describe both archaeological sites and artefacts. Even if these terminology standards do not offer terms that are precise enough for a specialist's needs they provide a good, generalised starting place. Additional keywords can be added to specify the precise subject in more specialised terms.

### 4.2.2  Spatial and temporal coverage

Others will need to know where and when on earth your data refer to, and you’ll no doubt need to keep detailed track of this for your own purposes too. It’s possible to identify the spatial and temporal location of your aerial photograph rectification in a number of ways, including text descriptions (e.g. placenames and temporal period names) and numeric descriptions (e.g. UTM coordinates, latitude and longitude, National Grid References).

General points to keep in mind when describing spatial and temporal locations include keeping track of the numeric location as well as a text description, as placenames are often repeated (e.g. Dublin, Ireland and Dublin, Ohio in the United States) and temporal names mean different things in different places (e.g. the ‘Roman’ period does not start until the late first century AD in Scotland).

For numeric descriptions of image location there must be provision of a valid geographical centre point, bounding box or polygon boundary description. It is important to label the x, y, and z coordinates clearly and specify the unit of measurement used. It’s also very helpful if you are able to indicate the precision with which you have recorded the spatial location.

### 4.2.3 Format

It is important to provide a description of the format of each file in your dataset is stored in and an overview of formats is provided in section 3.3 *Overview of data formats*. Appropriate formats for archiving digital datasets resulting from aerial photographs or remotely sensed images are discussed in section 5 *Archiving your data*.

### 4.2.4 Rights management

All information users need accurate information about copyright restrictions that relate to a data resource. Clear indication of who controls copyright on all aspects of the information contained within a digital file is especially important. If you re-use digital data for which you do not own the copyright, you should indicate this and refer potential users to any documentation that describes who can and can not access and use the information. For example, if you have used a SPOT satellite image as part of a GIS project it may well be a violation of your licence from SPOT to share the original satellite image with anyone else.

### 4.2.5 Creator

The term ‘creator’ can be a bit misleading, because often no single person can be credited with primary intellectual responsibility for a digital resource. Instead it is helpful to keep track of anyone whose involvement helped produce the digital dataset. This includes information about the funding agency or developer who paid for the images/interpretation/research, the company or organisation responsible for production of the source image, pilots, photographers, rectifiers, image processors, project managers, and others. However, don’t get too carried away and list every person who walked into the room where the digital dataset was being created, but rather choose the people and organisations most important in helping to create and maintain the data. At a minimum, the data provider and creator of the metadata should be entered here.

### 4.2.6 Date

There are many different kinds of dates that are important in the life cycle of a digital dataset related to aerial photography and remote sensing. Despite this, the date field should only refer to the date of image capture. Dates referring to the content of the digital file — for example the archaeological period in which a monument was built — are best described under the heading of spatial and temporal coverage. Any other date information, including interpretation date, documentation date, publication date, and archiving date, should be placed within the processing log.

The International Standards Organisation has made a recommendation for the best way to record dates in [ISO8601](http://www.iso.org/iso/catalogue_detail?csnumber=40874). Their recommendation is that dates be identified either in the format YYYY or YYYY-MM-DD where YYYY is the year, MM is the month, and DD is the date. In some cases the exact time an image was acquired may be relevant, for example when it is important to minimise shading in a satellite image; please record this information too.

### 4.2.7 Relation
Any text or number code which is used to identify a resource uniquely should be recorded. Examples include image or photographic frame numbers from commercial data suppliers, internal project identification numbers, and accession numbers issued by archives, libraries, museums, the National Monuments Record (NMR), and the regional Historic Environment Records (HERs) or Sites and Monuments Records (SMRs).

### 4.2.8 Instrumentation
Often a specific instrument is coupled with its own software or, in the case of aerial photography, a specialist camera may be associated with a calibration file (essential information for the rectification of distortion and other errors associated with a specific instrument and image). For the user of aerial photographic or remote sensing data it is essential to understand the limitations or characteristics associated with instrumentation; for the provider of such data it is therefore essential to record the instrument and any other relevant technical data.

Common instruments are SPOT (Satellite Pour l’Observation de la Terre) and Landsat.

* SPOT (e.g. SPOT Panchromatic, SPOT XS, SPOT 5) is a remote sensing satellite which has been developed by the French National Space Centre (CNES). The first SPOT (SPOT 1) was launched in February 1986, SPOT 2 was launched in 1988.
* Landsat (e.g. Landsat MSS and Landsat TM) is another series of satellites that produce images of the earth. The Landsat remote sensing satellite program was developed by NASA (National Aeronautics and Space Administration). Landsat data are provided in .BIL (band interleaved by line) or .BIP (band interleaved by pixel) formats.

Other common instrument types include:

* KVR 1000
* MK4
* KFA (1000/3000)
* Shuttle Oblique Photography
* Radarsat / Radarsat – Stereo
* ERS 1/2
* Carterra 1
* Earlybird
* Quickbird
* Orbview 3
* HSI
* Aries 1

### 4.2.9 Resolution

Most remote sensing data are collected and supplied in digital raster format. This means that each single digital number represents one observation of a piece of the earth’s surface. The size and shape of this area is the spatial resolution. Resolution is related to scale and precision (quantifying the size and location of the smallest feature that can exist in the data), but not to accuracy (indicating whether a specific stated size or location is in fact correct). Information about resolution is important as it implicitly specifies both the geographic precision and the size of archaeological features that one can reasonably expect to discover in the data.

Although in some circumstances you can specify the resolution of a dataset with just one figure (’25 metres’ would indicate that both the X- and the Y-resolution are 25 metres), good practice requires that you give separate X and Y resolutions. A single resolution figure is often insufficient for a variety of reasons:

* Depending on the instrument or sensor used, resolution may be the same for all the pixels (picture elements) in an image, or it may vary depending on the angle and distance between the instrument and the ground. Resolution is indicated by giving horizontal size (across track) and a vertical size (along track) of a pixel, which can be in metres or in arc seconds. Pixels can be (extremely) elongated, as in high-resolution RS data collected by low-flying aircraft. There are other common distortions to the stated resolution in such data but you can often account for these simply by specifying the instrumentation (see above).
* For photographic originals that are being converted to a digital format by scanning, the software can be configured to result in different X and Y resolutions.

Remember, any geometric transformation (such as georeferencing) or image enhancing technique (such as filtering) that is applied to a digital dataset may result in altered resolution settings which may bear no direct relation with the resolution of the original. If precise information about resolution is unobtainable, it will help if you can provide data about the instrument height, and scale of original (as in APs), etc.

As many general purpose scanners apply false (interpolated) resolution rather than true (optical) resolution, it is often wise to document the scanner used and the scanning resolution. Scanning resolution is generally specified as dots per inch or lines per inch.

### 4.2.10 Processsing log

There are three main categories of information about processing that are important to document: pre-processing, cleaning, and rectification. For all items listed in a processing log it is generally a good idea to indicate clearly what software was used, giving the full name and version numbers, and when the major processing steps took place.

‘Pre-processing’ usually encompasses any processing step that is performed in order to get digital data into a useful form for analysis and interpretation to begin. There is such huge variation in how this can be done that it is impossible to provide a complete list of options here. In general, though, it is important to document:

* Description of the original image
* A list of all steps leading to the production of the digital version
* Final image type
* Final format in which the image is held

When documenting procedures relating to the cleaning of digital remote sensing data, you may wish to include:

* A list of software used – it’s generally a good idea to specify the precise version
* A description of all radiometric corrections
* A description of all destriping activities
* A description of all noise reduction or despiking activities

Finally, it is important to document all processes carried out while rectifying or georeferencing digital image files. This requires you to:

* Specify ‘target’ coordinate points
* Note how you established the coordinates of the control points. Control point information may be obtained from field measurements (for instance by GPS), from maps, or from other images
* Describe the rectification method and transformation type you used, and the resulting error. Many methods are available and each carries its own set of advantages and disadvantages. Each carries some unavoidable error, and this should be documented.

### 4.2.11 Type

It’s a good idea to keep a technical description of each image that you work with. The following table summarises the major types of images available in aerial photography and remote sensing.

* Aerial Photography – generally types are variations on vertical or oblique photographic formats.
    * Oblique Panchromatic / Panchromatic – Stereo
    * Oblique Colour / Colour – Stereo
    * Oblique FC / FC – Stereo
    * Vertical Panchromatic / Panchromatic – Stereo
    * Vertical Colour / Colour – Stereo
    * Vertical FC / FC – Stereo
    * Other (please specify)
* Remote Sensing – airborne remotely sensed data are generally provided in digital form and normally come on magnetic tape, magnetic disk or optical media such as CD-ROM. Depending on the instrument, there may be several planes of information representing different spectral bands.
    * Multispectral Scanner
    * Thermal Linescanner
    * Videography
    * Digital photography
    * Oblique Satellite Photography – Panchromatic / Panchromatic Stereo
    * Oblique Satellite Photography – Colour / Colour Stereo
    * Vertical Satellite Photography – Panchromatic / Panchromatic Stereo
    * Vertical Satellite Photography – Colour / Colour Stereo
    * Satellite Panchromatic Digital
    * Satellite Multispectral Scanner Digital
    * Satellite RADAR / RADAR – Stereo / RADAR – Polarimetry
    * Other (please specify)

### 4.2.12 Legend

All interpretations based on aerial photography or remotely sensed data require documentation about the graphical conventions used. Graphical data are generally devalued if a legend is not supplied, or if it is inadequate or misleading. It’s well worth spending some time thinking about the kinds of information to include in your legend. In most cases this should not be an arduous task and it will generally allow you to organise and interpret your own data in a more efficient manner. Some organisations provide lists of standard conventions which can be adhered to when graphical output is generated.

Begin your legend with a descriptive title. In some cases this may be all that is required. This may occur when you are working with a scanned air photograph as it is unlikely to need an extensive legend because information on its geographic location, resolution, source, and image type is held elsewhere in your documentation.

Generally, though, every image should have an authoritative legend. In most instances these legends will still be very simple. For example, with categoric data you will need to document the numeric value, colour coding, shading, symbols or stippling associated with specific features. Although in many cases a simple description of a colour code may be sufficient, you should be aware that colours may display differently on individual computer screens.

More complex situations may also emerge. In the case of multi- or hyper-spectral imagery from non-standard sensors it may well be necessary to provide an extensive legend specifying what each band represents.

Legends may need to reflect the complexity of software used to provide data, or the data structure associated with specialist software. If an aerial photograph interpretation, for example, has been created in a CAD system the legend must reflect the fact that the information may be divided between separate layers representing specific themes. Each layer may be associated with a separate set of graphical conventions used to discriminate between specific objects or types of features. Clearly in this instance a nested legend describing individual layers and their associated conventions may be necessary. Alternatively, an image may have been prepared within a GIS which has the capability of attaching multiple text or numeric attributes through an associated table or database. Suitable documentation would include a description of the database structure, including any coding or related information needed to use the graphical database.

### 4.2.13 Bibliography

It is often useful to keep track of bibliographic references of relevance to the origin, processing or interpretation of the digital resource. The Harvard System is recommended as this is commonly used in archaeology.
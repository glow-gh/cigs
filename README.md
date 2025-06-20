# CIGS

Cuneiform Inscriptions Geographical Site Index

### Summary 
The *Cuneiform Inscriptions Geographial Site* (CIGS) index contains a basic set of primary spatial, toponym, attribute, and external link information on more than 500 archaeological locations where texts written in cuneiform and derived scripts have been found. In use across the wider Middle East from c. 3,400 BCE until 100 CE, cuneiform is one of the earliest scripts and most extensively documented ancient scripts in world history. This resource has been prepared by researchers of the [Department of Linguistics and Philology](lingfil.uu.se) of [Uppsala University](uu.se). The index is intended as a tool for students and researchers in cuneiform studies and related areas and as an aid to cultural heritage managers and educators in communicating and safeguarding this unique body of world written heritage. The index remains under development and is regularly updated. The authors will very much appreciate notices of any omissions, errors, or inaccuracies. For any inquiries, please contact [Rune Rattenborg](https://www.katalog.uu.se/profile/?id=N18-1120) ([rune.rattenborg@lingfil.uu.se](mailto:rune.rattenborg@lingfil.uu.se)).

### Formal
Versions v.0.x, released as the _Cuneiform Site Index_ (CSI), were prepared by Rune Rattenborg and [Memories For Life: Materiality and Memory of Ancient Near Eastern Inscribed Private Objects](https://www.lingfil.uu.se/research/assyriology/current-projects/), a project funded by the [Swedish Research Council](https://www.vr.se) (grant no. [2016-02028](https://www.vr.se/swecris#/project/2016-02028_VR)). Versions v.1.x and higher are released as _Cuneiform Inscriptions Geographical Site_ (CIGS) index and prepared by the individual authors mentioned below and [Geomapping Landscapes of Writing (GLoW): Large-scale Spatial Analysis of the Cuneiform Corpus (c. 3400 BCE to 100 CE)](https://www.lingfil.uu.se/research/assyriology/glow/), a project funded by [Riksbankens Jubileumsfond](https://rj.se) (grant no. [MXM19-1160:1](https://rj.se/en/grants/2019/geomapping-landscapes-of-writing-glow-large-scale-spatial-analysis-of-the-cuneiform-corpus-c.-3400-bce-to-100-ce)). Release formats are (as of v.0.1) .geojson, .kml, and .csv. All resources are released under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/) ([https://creativecommons.org/licenses/by-nc-sa/4.0/](https://creativecommons.org/licenses/by-nc-sa/4.0/)). The index and its application is described in more detail in [Rattenborg et al. (2021) “An Open Access Index for the Geographical Distribution of the Cuneiform Corpus”](https://cdli.mpiwg-berlin.mpg.de/articles/cdlj/2021-1). 

Please cite as: Rattenborg, Rune; Carolin Johansson, Nils Melin-Kronsell, Seraina Nett, Gustav Ryberg Smidt, Jakob Andersson. 2022. "Cuneiform Inscriptions Geographical Site Index (CIGS)". v.1.5. Zenodo, 16 November 2022. 

### Version history

version | date | online release | description
:---:|:-----|:---:|:--------------------
v. 0.1 | November 2019 | 01/11/2019|247 entries and 14 fields (see data specification below)
v. 1.0 | October 2020|01/10/2020 | 334 entries and 19 fields (working file submitted to [Cuneiform Digital Library Initiative](http://cdli.mpiwg-berlin.mpg.de) (CDLI), not public download)
v. 1.1 | December 2020 | 01/12/2020 | 367 entries and 18 fields (see data specification below)
v. 1.2 | May 2021 | 01/05/2021 | 553 entries and 19 fields (see data specification below)
v. 1.3 | July 2021 | 01/07/2021 | 562 entries and 19 fields (see data specification below)
v. 1.4 | November 2021 | 01/11/2021 | 564 entries and 25 fields (see data specification below)
v. 1.5 | November 2022 | 01/11/2022 | 579 entries and 26 fields (see data specification below)
v. 1.6 | July 2023 | 01/07/2023 | 597 entries and 26 fields (see data specification below)
v. 1.7 | December 2024 | 31/12/2024 | 598 entries and 26 fields (see data specification below)

### Index field categories
The index contains a total twenty-six fields, including one primary ID, one integer field for accuracy, twenty-two string fields with toponyms and links, and two spatial data fields. Index fields include **site_id (str), accuracy (int), cdli_provenience_id (str), anc_name (str), transc_name (str), ara_name (str), arm_name (str), fas_name (str), geo_name (str), gre_name (str), heb_name (str), rus_name (str), legacy_name (str), pleiades_url (str), osm_url (str), geonames_url (str), wik_en (str), wik_ara (str), wik_fas (str), wik_gre (str), wik_heb (str), wik_tr (str), rla_url (str), wikidata_url (str), lon_wgs1984 (dbl)** and **lat_wgs1984 (dbl)**. Coordinates given use the WGS 1984 geographic coordinate reference system ([EPSG 4326](https://epsg.io/4326)) and have been truncated to four decimal digits. Site locations have been traced from archaeological gazetteers and web mapping services (e.g. [Pleiades](https://pleiades.stoa.org), [GeoNames](https://www.geonames.org) and [OpenStreetMap](https://www.openstreetmap.org)) and digitally generated from optical recognition using current and legacy satellite imagery datasets in QGIS 3.x. Below is a description of the individual data fields contained in this index.

field | type | description
:----|:----:|:--------------------------------
site_id | str | Primary ID. Each record is identified with a unique three-letter code.
accuracy | int | A formal assessment of the level of geographical accuracy with which position given can be said to relate to the historical location in question on a four-tier scale, 3 being certain, 2 being representative, 1 being tentative, and 0 being unknown. 
cdli_provenience_id | str | The numerical provenience ID for the corresponding site in the [Cuneiform Digital Library Initiative](http://cdli.mpiwg-berlin.mpg.de) (CDLI) catalogue, if available. As of v.1.7, this value is supplied as a stable URL using http://cdli.mpiwg-berlin.mpg.de/proveniences/[cdli_provenience_id]
anc_name | str | Common rendering of the ancient name of the site in question, if known, based on readings from cuneiform texts.
transc_name | str | The transcribed name of the site as drawn from the principal language of the national entity currently associated with the record in question. Unless originating from a Latin script, the source of the transcription will be contained in either of the name fields given below, using Romanization conventions given by the [American Library Association and the Library of Congress (ALA-LC)](https://www.loc.gov/catdir/cpso/roman.html).
ara_name | str | Arabic name of the site, if applicable and available.
arm_name| str | Armenian name of the site, if applicable and available.
fas_name | str | Farsi name of the site, if applicable and available. 
geo_name | str | Georgian name of the site, if applicable and available.
gre_name | str | Greek name of the site, if applicable and available. 
heb_name | str | Hebrew name of the site, if applicable and available. 
rus_name | str | Russian name of the site, if applicable and available.
legacy_name | str | Concatenated character string values for corresponding provenience(s) from [Cuneiform Digital Library Initiative](http://cdli.mpiwg-berlin.mpg.de) and various other data sources.
pleiades_url | str | The stable URL of a corresponding place record in [Pleiades: A Gazetteer of Ancient Places](https://pleiades.stoa.org), if available.
osm_url | str | The stable URL of a corresponding place record in [OpenStreetMap](https://www.openstreetmap.org), if available.
geonames_url | str | The stable URL of a corresponding place record in [GeoNames](https://www.geonames.org), if available.
wik_en | str | URL of corresponding article on [Wikipedia](https://en.wikipedia.org), if available.
wik_ara | str | URL of corresponding article on [ويكيبيديا](https://ar.wikipedia.org/), if available.
wik_fas | str | URL of corresponding article on [ويکیپديا](https://fa.wikipedia.org), if available.
wik_gre | str | URL of corresponding article on [Βικιπαίδεια](https://el.wikipedia.org/) if available.
wik_heb | str | URL of corresponding article on [ויקיפדיה](https://he.wikipedia.org/) if available.
wik_tr | str | URL of corresponding article on [Vikipedi](https://tr.wikipedia.org/) if available.
rla_url | str | URL of the starting page of the corresponding lemma in the [Reallexikon der Assyriologie](https://rla.badw.de/das-projekt.html) as publicly available from the [Bayerische Akademie der Wissenschaften](http://publikationen.badw.de/de/rla/).
wikidata_url | str | The stable URL of the corresponding [Wikidata](https://www.wikidata.org) record, if available.
lon_wgs1984 | dbl | Longitude of the record location in decimal degrees in the WGS 1984 geographic coordinate reference system (EPSG 4326).
lat_wgs1984 | dbl | Latitude of the record location in decimal degrees in the WGS 1984 geographic coordinate reference system (EPSG 4326).




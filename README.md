<a href="https://juncture-digital.org"><img src="https://juncture-digital.org/images/ve-button.png"></a>

<param ve-config 
       title="DH Lab Fall 2022 Workshop"
       author="Ann Hanlon"
       banner="https://upload.wikimedia.org/wikipedia/commons/4/44/NASA%E2%80%99s_Webb_Reveals_Cosmic_Cliffs%2C_Glittering_Landscape_of_Star_Birth.jpg"
       layout="vertical">

<!-- Entities discussed throughout the essay are typically defined before the essay text and
     are thus available in all text.  Entity identifiers (QIDs) can be found in either
     Wikipedia or Wikidata (https://www.wikidata.org)> -->
<param ve-entity eid="Q186447"> <!-- James Webb Space Telescope -->
<param ve-entity eid="Q50042"> <!-- Carina Nebula -->
<param ve-entity eid="Q62706"> <!-- Johann Baptist Homann -->
<param ve-entity eid="Q537520"> <!-- James E. Webb -->
<param ve-entity eid="Q207383"> <!-- South Orkney Islands -->


# Introduction

This is a sample visual essay to demonstrate how to use Juncture to build visual essays. The banner image features one of NASA's images from the James Webb Space Telescope, showing the edge of the Carina Nebula [^1]. Here, the first image is a much earlier rendition of a more nearby celestial phenomenon, the movement of the planets. This is from the UWM Libraries American Geographical Society Library digital collection featuring the Atlas Novus Coelestis, from 1742. https://collections.lib.uwm.edu/digital/collection/celestial/id/81/rec/13
<param ve-image 
       manifest="https://collections.lib.uwm.edu//digital/iiif-info/agsnorth/2574/manifest.json">

# Basic usage
       
## Port au Prince: IIIF image "to fit"

From the Smithsonian Institution collections - small boats in harbor at Port au Prince, 1923-24. This image uses the fit=contain parameter to make sure the default view is the entire image. You can find the record here: [https://collections.si.edu/search/detail/edanmdm:siris_sic_13621](https://collections.si.edu/search/detail/edanmdm:siris_sic_13621)
<param ve-image fit="contain"
       manifest="https://ids.si.edu/ids/manifest/SIA-SIA2010-0721">

## Image without zoom

Globi Coelestis in Tabulis Tlanas Redacti Pars I: Full size with no zoom or fit="contain" code. https://collections.lib.uwm.edu/digital/collection/celestial/id/84/rec/22
<param ve-image  
       manifest="https://collections.lib.uwm.edu//digital/iiif-info/agdm/1435/manifest.json">
       
## Image with zoom
Globi Coelestis in Tabulis Tlanas Redacti Pars I0: Zoomed in using image coordinates to focus on a particular part of the image (in this case, an image of the "camelopardalus constellation).
<param ve-image region="2135,1939,706,586"
       manifest="https://collections.lib.uwm.edu//digital/iiif-info/agdm/1435/manifest.json">
       
## Image with zoom-to
In this image, you can also see part of the constellation <span data-click-image-zoomto="1496,1258,847,703">Cygnus</span>. You can also zoom in closer to view details of the image for constellation <span data-click-image-zoomto="3145,1878,2107,1750">Cephus</span>. 
<param ve-image  
       manifest="https://collections.lib.uwm.edu//digital/iiif-info/agdm/1435/manifest.json">
       
## Map image
You can use Juncture to great effect with images of maps. This is a nautical chart of South Orkney, dated 1847. It's very sparse, but you can zoom in to better view <span data-click-image-zoomto="1496,1258,847,703">Georgie du Sud and the Cape of Disappointement</span>. You can also veer south to better view <span data-click-image-zoomto="3145,1878,2107,1750">Coronation Island</span>. https://collections.lib.uwm.edu/digital/collection/agdm/id/21500/rec/4
<param ve-image  
       manifest="https://collections.lib.uwm.edu//digital/iiif-info/agdm/1435/manifest.json">

## Map

The South Orkney Islands are a group of islands in the South Atlantic Ocean. We are using the map information from Wikidata to create the map to right.
<param ve-map center="Q207383" zoom="11">

Lat/long based map - using decimal-based lat/long for Coronation Island
<param ve-map center="18.5425, -72.338611" zoom="10">


## Video

You can also include Youtube videos by using the param ve-video code and the youtube video ID. This is a TED-Ed video called "The first and last king of Haiti," by Marlene Daut, created in 2019.
<param ve-video id="q7lfSjjMNU8" title="The first and last kind of Haiti">

## Finding IIIF resources

This image is a page from a fourteenth century copy of Al-Sufi's "Book of the Constellations of the Fixed Stars," held by the National Library of France, and featured in the Library of Congress's [World Digital Library](https://www.loc.gov/collections/world-digital-library/about-this-collection/) collection. [*Al-Sufi's "Book of the Constellations of the Fixed Stars," followed by Maxims, and al-Qazwini's "The Wonders of Creation".*](https://lccn.loc.gov/2021667391)
<param ve-image 
       manifest="https://www.loc.gov/item/2021667391/manifest.json)">
       
       
       
# References

[^1]: Image: National Aeronautics and Space Administration  (a U.S. federal government agency; [https://www.nasa.gov/](https://www.nasa.gov/), Public domain, via [https://commons.wikimedia.org/wiki/Main_Page](Wikimedia Commons)

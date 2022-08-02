<a href="https://juncture-digital.org"><img src="https://juncture-digital.org/images/ve-button.png"></a>

<param ve-config 
       title="CLACS Summer 2022 Workshop"
       author="Ann Hanlon"
       banner="https://iiif.juncture-digital.org/banner/?url=https://upload.wikimedia.org/wikipedia/commons/f/f7/Citadelle_Laferri%C3%A8re%2C_Haiti%2C_1920_-_49810176056.jpg"
       layout="vertical">

<!-- Entities discussed throughout the essay are typically defined before the essay text and
     are thus available in all text.  Entity identifiers (QIDs) can be found in either
     Wikipedia or Wikidata (https://www.wikidata.org)> -->
<param ve-entity eid="Q206194"> <!-- Citadelle Laferrière -->


# Introduction

This is a sample visual essay to demonstrate how to use Juncture for the CLACS 2022 Summer Workshop. The banner image features Haiti's Citadelle Laferrière, photographed from an airplane in 1920[^1]. The first image featured in this essay is also an image of Citadelle Laferrière, from 1935.
<param ve-image 
       manifest="https://collections.lib.uwm.edu//digital/iiif-info/agsnorth/2574/manifest.json">

# Basic usage
       
## Port au Prince: IIIF image "to fit"

From the Smithsonian Institution collections - small boats in harbor at Port au Prince, 1923-24. This image uses the fit=contain parameter to make sure the default view is the entire image. You can find the record here: [https://collections.si.edu/search/detail/edanmdm:siris_sic_13621](https://collections.si.edu/search/detail/edanmdm:siris_sic_13621)
<param ve-image fit="contain"
       manifest="https://ids.si.edu/ids/manifest/SIA-SIA2010-0721">

## Image without zoom

Carte de l'Isle Saint-Domingue..., 1730: Full size with no zoom or fit="contain" code.
<param ve-image  
       manifest="https://collections.lib.uwm.edu//digital/iiif-info/agdm/1435/manifest.json">
       
## Image with zoom
Carte de l'Isle Saint-Domingue..., 1730: Zoomed in using image coordinates to focus on a particular part of the image (in this case, an image of a map).
<param ve-image region="2135,1939,706,586"
       manifest="https://collections.lib.uwm.edu//digital/iiif-info/agdm/1435/manifest.json">
       
## Image with zoom-to
In this map, you can also see the island of <span data-click-image-zoomto="1496,1258,847,703">Inague</span>, to the east of Cuba. Further to the east is the western tip of <span data-click-image-zoomto="3145,1878,2107,1750">Puerto Rico</span>. 
<param ve-image  
       manifest="https://collections.lib.uwm.edu//digital/iiif-info/agdm/1435/manifest.json">

## Map

The Citadelle Laferrière is several miles inland from Cap-Haitien. We are using the map information from Wikidata to create the map to right.
<param ve-map center="Q206194" zoom="11">

A map based on latitude and longitude
<param ve-map center="32.262084, 64.391554" zoom="2.5" stroke-width="0" show-labels>
	<param ve-map-layer geojson url="/geojson/peony.json" title="Peony Distribution" active> 

## Video

You can also include Youtube videos by using the param ve-video code and the youtube video ID. This is a TED-Ed video called "The first and last king of Haiti," by Marlene Daut, created in 2019.
<param ve-video id="q7lfSjjMNU8" title="The first and last kind of Haiti">

## Finding IIIF resources

This object is from the National Archives of Haiti, and is found in the Library of Congress's [World Digital Library](https://www.loc.gov/collections/world-digital-library/about-this-collection/) collection. *The Laws of the French Colony of Saint-Domingue.* Cap-Français: P. Roux, -07 to -08, 1801, [https://www.loc.gov/item/2021666967/](https://www.loc.gov/item/2021666967/).
<param ve-image 
       manifest="https://www.loc.gov/item/2021666967/manifest.json">
       
## Multiple pages in a IIIF object

This object from the Harvard University Digital Collections is a book with multiple pages. You can identify a specific page to focus on by using the "seq" tag after the manifest address. 
<param ve-image 
       manifest="https://iiif.lib.harvard.edu/manifests/drs:492788288" seq="5">
       

       
# References

[^1]: Citadelle Laferrière, Haiti, 1920, Archives Branch, USMC History Division, CC BY 2.0, via [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Citadelle_Laferri%C3%A8re,_Haiti,_1920_-_49810176056.jpg)

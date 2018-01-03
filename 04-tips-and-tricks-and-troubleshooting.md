# Tips and Tricks and Troubleshooting

> In this section we will go over some of advanced features as they pertain to specific areas of using an app.

## Custom Map Sources {#customMapSources}

In addition to built-in online raster maps, Galileo Offline Maps also supports custom online maps. You can add any map source you like using a special XML file that contains description of map provider.

### Simple custom map sources {#simpleCustomMapSources}

The following example shows how the XML file for OpenStreetMap source may be defined:

```
<?xml version="1.0" encoding="UTF-8"?>
<customMapSource>
<name>OpenStreetMap</name>
<url>http://{$serverpart}.tile.openstreetmap.org/{$z}/{$x}/{$y}.png</url>
<serverParts>a b c</serverParts>
</customMapSource>
```

### Custom multi-layer map sources {#customMultiLayerMapSources}

Map sources which consist of two or more layers can be defined, similar to single-layer custom map sources. The following example shows how the XML file for OpenSeaMap hybrid source may be defined:

```
<?xml version="1.0" encoding="UTF-8"?>
<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<customMapSource>
<name>OpenSeaMap</name>
<minZoom>0</minZoom>
<maxZoom>18</maxZoom>
<layers>
<layer>
<url>http://{$serverpart}.tile.openstreetmap.org/{$z}/{$x}/{$y}.png</url>
<serverParts>a b c</serverParts>
</layer>
<layer>
<minZoom>9</minZoom>
<maxZoom>18</maxZoom>
<url>http://tiles.openseamap.org/seamark/{$z}/{$x}/{$y}.png</url>
</layer>
</layers>
</customMapSource>
```

The most important tags of this definition are described below:

&lt;name&gt; – the name of the map source,

&lt;url&gt; – the path for the tiles of the map source with the specific placeholders in curly brackets:

* {$z} – the zoom level,  
* {$x} – the X tile coordinate,  
* {$y} – the Y tile coordinate,  
* {$invX} – the inverted X tile coordinate,  
* {$invY} – the inverted Y tile coordinate,  
* {$serverpart} – \(optional\) in case of multiple servers for the map source.  
* &lt;serverParts&gt; – a space-separated list of parts that replace the {$serverpart} in &lt;url&gt; tag.  
* &lt;retina&gt; – tag for defining the size of Retina map tiles:

* &lt;retina&gt;1&lt;/retina&gt; – for 512х512 px \(e.g. Google Maps HD\),
* &lt;retina&gt;2&lt;/retina&gt; – for 256х256 px \(e.g. CloudMade HD\).

#### How to add

There are several ways to add custom online map source to the app:
1. Place the XML file in the app shared folder in iTunes.
2. Open the XML file attached in Email on your device using the "Open in Galileo" option.
3. Open the XML file from Dropbox on your device using the "Open in.." option.
	
As a result, the new map source will appear in Map Source list.

#### Troubleshooting

Sometimes you can see empty map areas (tiles), with the following warning messages on the map:
* "Tile loading error. Please check your Internet connection" – this appears when tiles are missing in the cache and app can't download them. Enable an Internet connection or go to ’online’ mode to load the missing tiles.
* "Tile loading error. Wrong response from the server" – the online server is not responding. Try to navigate to this area later to reload any missing tiles.

## Offline Maps Import {#offlineMapsImport}

Feature, available as an in-app purchase, allows you to import previously created custom offline maps in .sqlitedb or .mbtiles format.

#### Creating an offline map

The main idea is to create an offline map for the desired area in advance with one of the following tools on your computer using one of the following tools:

* [Mobile Atlas Creator](http://mobac.sourceforge.net/) (known also as MOBAC)
* [TileMill](https://tilemill-project.github.io/tilemill/)
* [SAS.Planet](http://sasgis.ru/sasplaneta/)

_Mobile Atlas Creator (MOBAC)_ – is free software that allows you to download maps from numerous map sources, and save them in the .sqlitedb format used by Galileo Offline Maps. This tool is compatible with Windows, Mac OS X and Linux.

Reference: to learn how to create offline maps in **.sqlitedb** format, please refer to the [MOBAC manual](http://mobac.sourceforge.net/quickstart/).
				
_TileMill (by MapBox)_ – is a desktop application for cartographers to quickly and easily design and create stunning offline maps in the .mbtiles format supported by Galileo Offline Maps. It is completely compatible with Mac OS X, Windows and Ubuntu.

Reference: to learn how to create offline maps in **.mbtiles** format, please refer to the [TileMill manual](https://tilemill-project.github.io/tilemill/docs/manual/).
					
SAS.Planet – is a program designed for viewing and downloading high-resolution satellite imagery and conventional maps in .sqlitedb format.
Reference: to learn how to create offline maps in **.sqlitedb** format, please refer to the [SAS.Planet manual](http://www.sasgis.org/wikisasiya/doku.php).

#### Importing offline maps

Once you have created an offline map, you should upload it to your device. There are two ways to import an offline map into your device: via iTunes or Dropbox.

#### Using offline maps

Go to Map Source in app settings and select the imported map name in the list and back to the map view. If you are not over the area with offline map, tap the green arrow indicating the direction to the offline map. Zoom in to see a detailed view of your offline map.
						
#### Troubleshooting

Sometimes you can see empty map areas, with the following warning messages on the map:
						
"Tile is not in your offline map. Please add more layers." – this means that there are no map tiles on the current zoom level in your offline map. You have probably imported insufficiently detailed levels, so when you zoom in there are no downloaded tiles for that level.

## MIUI users troubleshooting {#MIUI}

#### Xiaomi and other MIUI phones issue

MIUI by default doesn’t let apps in the background access GPS, which is what causes this issue.

Here’s what you need to do to solve the problem:

* Pull down toggle bar.
* Hold the GPS icon to reach GPS settings.
* Here, change Location mode to High accuracy

To make sure the app isn’t killed while in background go to Settings  > Battery & performance > Manage app battery usage, now disable/turn off Power saving mode or add Galileo to battery saver exceptions, by clicking Choose apps > Galileo > No restrictions.
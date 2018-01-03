 # Settings

> Galileo Offline Maps is available in a ready-to-use state and app settings should be considered as optional and more advanced way of using the app. Settings lets you configure app options, purchase additional features and manage geo data representation.

## Map Sources {#MapSources}

To switch to another map to display, select **Map Source** menu in app settings. There are two types of maps you can use within the app: offline and online maps.

### Offline maps
						
Vector map source is set by default. Once you’ve downloaded it (**internet connection required**), it will be available offline.
Vector maps are detailed, smooth, fast and provide high quality image rendered in real time on the device. It takes up less storage space than raster maps.

**Note**: you can also use your own maps in .sqlitedb and .mbtiles formats, previously created on computer and then imported into your device. Such maps can be viewed offline even when your mobile device has no internet connection.

	 						 						
### Online maps
						
There is a list of built-in raster map sources available online:
				 						
* HikeBikeMap
* Humanitarian OSM
* OpenBusMap
* OpenCycleMap
* OpenStreetMap
* Stamen – Terrain (USA only)
* Stamen – Toner
						 						
Caching is always enabled – the app saves all recently viewed map images in your cache and keeps them available for offline usage. To save maps, navigate to the area you are going to visit and zoom-in while you have access to the Internet.
						 						
**Note**: map download speed can vary while using an online sources, and depends on the speed of your Internet connection and the speed of the server from where the map is downloaded.

In addition to built-in online raster maps, Galileo Offline Maps also supports custom online maps. You can add any map source you like using a special XML file that contains description of map provider.

## Vector Maps Settings

This section describes the vector maps related settings within the app.

### Download Maps

Vector maps are available and free for download within the app:
 
![](/assets/)

To **download a map of the selected country** tap the ![](/assets/) button next to the country name in Available Maps list.
To **pause a download**, tap the cell with the country name tap it again to resume a download,
To **go to downloaded map** tap the  button,
to **remove a map** swipe your finger across the country name from right to left, then tap the Delete button, or use the Edit button.

As OpenStreetMap data is constantly updated by thousands of volunteers around the world, map updates are available from time to time within the app. In Galileo app all vector map updates are free and distributed automatically. If there is an update for downloaded map, you will see Update button near the downloaded map name:

![](/assets/)

To **update all your downloaded maps** tap the “Update All” button.

![](/assets/)


### Font and Languages {#fontsAndLanguages}

#### Font size 

You can configure Galileo to display all text on a vector map at a comfortable font size. To increase, decrease, or change the default font size, go to app Settings > Font and Languages.

#### Preferred language order

In some regions objects on the map in addition to local names have names in other languages. Map will show the names on the first language in this list if exists. It may be useful for multilingual countries, such as Belgium where Dutch, French and German share official language status.


![](/assets/fonts_and_language.png)


### Map Features {#mapFeatures}

In addition to the basic appearance settings, you can select the objects you wish to display on the vector map. Select only the objects that you want to display to keep the map tidy and uncluttered:

* Restaurants, cafes, fast foods
* Bars, pubs, clubs
* Beauty salons, hairdressers
* Entertainment, arts and culture
* Monuments, places of worship
* Tourist attractions
* Hotels, hostels, campsites
* Banks, ATMs, currency exchanges
* Parking, gas and service stations
* Hospitals, clinics, pharmacy
* Shopping malls, supermarkets
* Police, post offices, embassies
* Universities, colleges, schools
* Public transport stops
* Train and metro stations
* Building names and numbers


## Appearance Settings {#appearance}

The following group of settings is used to configure how the main map looks.  

### Show Trip Monitor {#showTripMonitor}
 
To hide trip monitor panel from the map view, turn off this option.

### Show Coordinates {#showCoordinates}

To enable the real-time display of coordinates on the map, turn on this option. If enabled, crosshairs will appear in the center of the map and coordinates for the crosshairs will be beneath the map scale bar in selected format as well as the current zoom level:

![](/assets/show_coordinates.png)


### Show Zoom Buttons {#showZoomButtons}

To make visible zoom control buttons on the map, turn this option on. If enabled, plus and minus zoom buttons will appear on the map:

![](/assets/zoom_buttons.png)

### Show Bookmark Name

To make visible bookmark name on the map, turn this option on. If enabled, bookmark will change its view and the name of bookmark will appear:

![](/assets/)

### Screen Auto-Lock {#screenAutoLock}

The screen of your device will be turned off automatically after a specified period of time to save on power.
Turn this option off if you want your device not to lock the screen while using the Galileo app.


### Default Styles {#defaultStyles}

To set a color for GPS tracks and category for bookmarks used by default, go to app Settings &gt; Default Styles.  

#### Default track style

Selected style is a default line style for the newly recorded and imported GPS tracks:

_1. By color:_

![](/assets/default_styles_1.png)

_2. By speed:_

![](/assets/default_styles_2.png)

_3. By altitude:_

![](/assets/default_styles_3.png)

#### Default bookmark category

Selected category is a default icon for newly created and imported bookmarks:

![](/assets/default_styles.png)

## Advanced Settings {#advanced}

### Sync {#sync}

Galileo Offline Maps allows you to synchronize all your data to make your collections visible and available through all your devices using your Facebook or Google account.
App uses Facebook/Google login only for authentication, this does not let the Galileo post or share your data.
To enable synchronization feature, go to the app Settings > Sync and select the appropriate way to authenticate.
Note: use the same login on all your devices to keep the data synchronized. 
**Tip**: synchronization is a beta feature, so we recommend to backup your collections in advance to avoid unexpected data loss.

![](/assets/sync.png)


### Navigation {#navigation}

The default language of voice instructions you hear while navigating a route depends on the language your device is set to use. 
To change the language, select one from the Voice Instructions list:

![](/assets/settings_navigation_language.png)

**Note**: as the app use text-to-speech (TTS) engine instead of pre-recorded audio, correct pronunciation depends on the TTS engine.


### Data Backup {#dataBackup}

Backing up data is a great way to minimize accidental data loss and restore the most important geodata on your device.

#### Create backup

Tap Back Up My Collections button on Settings &gt; Data Backup screen to backup the collections within the app.  
**Note**: created backup only includes data from My Collections \(bookmarks and GPS tracks\), and it doesn't include downloaded and cached tiles.  
When the backup finished successfully, you'll see the name of the device along with the date and time the backup was created:

![](/assets/backup.png)

#### Save backup

Backups are stored on your device and will be removed automatically when the app is removed. To prevent data loss, we recommend to save your backups regularly.

You can use cloud services (Dropbox, OneDrive, Adobe Creative Cloud, Google Drive, etc) to save them.

![](/assets/backup_share.png)

#### Restore from a backup

There are several ways to restore your data from backup:

* Select .gbackup file from any file manager installed and choose Galileo:

![](/assets/open_backup_file_manager.png)

* Select item from your cloud service \(e.g. in Dropbox app\) and choose Galileo:

![](/assets/open_backup_dropbox.png)

* Move .gbackup file to Internal Storage &gt; Galileo\_backups folder. All .gbackup files from this directory will be listed in Galileo. Go to Settings &gt; Data Backup and tap prefered backup.

**Note**: restoring from backup will remove all current bookmarks and GPS tracks in My Collections.

### Cache info {#cacheInfo}

#### Map Refresh

To set how often to refresh cached map tiles, go to Settings &gt; Cache Info. All tiles older than selected time will be downloaded while browsing online.

![](/assets/cache_info.png)

#### Cache Info

All loaded map tiles will be automatically saved to your device's storage and can be managed in Settings &gt; Cache Info, so you can delete the tiles you no longer need if you want to free up storage space.


### Maps Storage {#mapsStorage}

If your device supporting SD Card memory extension and one of your storages become insufficient you can change default Map Download Storage in Settings &gt; Maps Storage. After selection one of the available storages all downloaded Maps will be moved to selected one. Maps will be downloaded on the storage with the largest amount of free space by default. If you don’t see Maps Storage Settings your device might not support SD Card memory extension or SD Card is not present.

![](/assets/maps_storage.png)

### GPS Filtering {#gpsFiltering}

Galileo Offline Maps app supports GPS data filtering in Settings &gt; GPS Filtering.  

#### Accuracy Threshold

Filter by the minimum accuracy at which the new points will be accepted. New points will be added to GPS track while recording if the accuracy is lower than selected (recommended value is 150 m).

![](/assets/accuracy_threshold.png)

**Example**: You are recording your GPS track while walking around your neighbourhood and you have entered a supermarket. Tall walls, roofs and other obstructions can block the signal from GPS satellites and the device cannot determine your location accurately enough. You may enable the accuracy filter to set the required accuracy and ignore inaccurate GPS data. If the received signal has lower than the required accuracy, that point will not be recorded in the track.

#### Distance Threshold

Filter by the minimum distance travelled before a new point will be recorded. New points will be added to GPS track while recording if the distance between them is greater than selected (recommended value is 5 m).

![](/assets/distance_threshold.png)

**Example**: You are recording your GPS track while jogging, then you meet a friend and stop to talk to him. As the GPS sends location coordinates every second, too many points will be recorded on the same spot while you are talking, and the recorded track will take up more space. You may enable the distance filter to ignore GPS points if they are too close to each other. New points will start recording as you exceed the distance selected in the filter.


### Units Format {#unitsFormat}

To set the units system and coordinates format you would like to use within the Galileo Offline Maps, go to Settings &gt; Units Format. 
 
#### Units system

The following units of measure for distance and speed are available to select from:

* **km** — for kilometres & km/h,
* **mi** — for miles & mph,
* **NM** — for nautical miles & kts.

#### Coordinates format

In Galileo Offline Maps you can choose to represent your coordinates in any way you like. The coordinate format you select will be used to display all coordinates within the app. Here is an example of different coordinate formats for New York city follows:

* +40.730598, -73.986580 \(DDD.DDDDD\)
* 40°43'50.1" N, 73°59'11.6" W \(DDD°MM' SS.S"\)
* 40°43.835' N, 73°59.194' W \(DDD°MM.MMM’\)
* 40.73060° N, 73.98658° W \(DDD.DDDDD°\)
* 18TWL 85577 09345 \(MGRS\)

## Help {#Help}


#### Contact Us

If you have faced a problem - here you can contact Support via email.


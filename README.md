# Airship-Pirates-Crafts
Datapacks for Airship Pirates Movecraft types.  Our layered setup requires a multitude of datapacks and require them to be loaded in the proper order.

## Setup
1. Start up your server with the datapacks present.
2. Disable each datapack by running the following commands in console:
```
datapack disable "file/AP-8.zip"
datapack disable "file/AP-7.zip"
datapack disable "file/AP-6.zip"
datapack disable "file/AP-5.zip"
datapack disable "file/AP-4.zip"
datapack disable "file/AP-3.zip"
datapack disable "file/AP-2.zip"
datapack disable "file/AP-1.zip"
datapack disable "file/AP-0.zip"
```
5. Enable each datapack by running the following commands in console:
```
datapack enable "file/AP-0.zip" after "file/movecraft-data.zip"
datapack enable "file/AP-1.zip" after "file/AP-0.zip"
datapack enable "file/AP-2.zip" after "file/AP-1.zip"
datapack enable "file/AP-3.zip" after "file/AP-2.zip"
datapack enable "file/AP-4.zip" after "file/AP-3.zip"
datapack enable "file/AP-5.zip" after "file/AP-4.zip"
datapack enable "file/AP-6.zip" after "file/AP-5.zip"
datapack enable "file/AP-7.zip" after "file/AP-6.zip"
datapack enable "file/AP-8.zip" after "file/AP-7.zip"
```

## Layered Setup
The datapacks are layered from 0 to 8 (currently) to allow us to use tags within tags (for example, `#ap_types:airship` is used in `#ap_types:factory`).  The `N` folder is used as a template for new layers.

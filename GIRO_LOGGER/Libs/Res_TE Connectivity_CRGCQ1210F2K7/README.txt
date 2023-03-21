
EE Concierge + Altium Library Install Instruction:

The following are the instructions for loading a library that was exported from EE Concierge into Altium.

The library will come as a zip file filled with all the necessary Altium data files required to load your EE Concierge parts into Altium. For every part there will be a pcb file, and a schematic file. There will also be an index file, a readme file, and finally the master library file itself. Do not try to open any of the individual part files, or the index file as they can't be loaded on their own.

Instead, to load a library you simply need to point Altium to this master library file named: 'EEConcierge.DbLib'. There are two ways to do this which we outline below. Whenever you need to load an updated version of your EE Concierge library the instructions are exactly the same. We've tagged the parts exports in such a way that Altium will overwrite and update any previously loaded parts as opposed to creating duplicates.

Method A:

1) Unzip the exported library
2) Double click on the file 'EEConcierge.DbLib'
3) Altium will open and load the library for you, you can now use your new components

Method B:

1) Unzip the exported library
2) Open Altium Designer
3) In the 'File' menu, click 'Open'
4) Browse to the unzipped library directory, select 'EEConcierge.DbLib' and click 'Open'


Altium will load the library, you can now use your new components
Part CRGCQ1210F2K7 (component id 2e3c324436ffef68) experienced an error during datasheet export:
Traceback (most recent call last):
  File "/usr/lib/python2.7/dist-packages/upconvert/writer/altium/altium.py", line 403, in export_component
    datasheets[datasheet_url] = self.save_datasheet(datasheet_url)
  File "/usr/lib/python2.7/dist-packages/upconvert/writer/altium/altium.py", line 287, in save_datasheet
    r.raise_for_status()
  File "/usr/lib/python2.7/dist-packages/requests/models.py", line 862, in raise_for_status
    raise HTTPError(http_error_msg, response=self)
HTTPError: 500 Server Error: Internal Server Error for url: https://www.te.com/commerce/DocumentDelivery/DDEController?Action=showdoc&DocId=Data+Sheet%7F1773204-3%7F1%7Fpdf%7FEnglish%7FENG_DS_1773204-3_1.pdf%7F4-2176347-788



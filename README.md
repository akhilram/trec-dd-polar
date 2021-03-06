TREC Dynamic Domain Polar Dataset
=================================
This is the dataset collected from a combination of Dr. Chris Mattmann's
[CSCI 572 Course at USC](http://sunset.usc.edu/classes/cs572_2015/).

The team list is generated using the following command:

``` ls | cut -d"-" -f2 | grep -v "json" | grep -v "py" | grep -v ade |
grep -v acadis | grep -v amd | uniq | sort ```

Contributing Teams 
================== 
* team1 
* team14 
* team16
* team18
* team22
* team24
* team29 
* team34 
* team36 
* team41 
* team42 
* team43
* team6

Additional Contributions 
======================== 
Dr. Mattmann's student,
[Angela Wang](https://github.com/snowangelwmy/), 
contributed 3 datasets. [2 crawls of ACADIS and one of
NASA AMD](https://github.com/snowangelwmy/csci572dr).

Dr. Mattmann himself also contributed a dataset crawl of [ADE](http://nsidc.org/acadis/search/), 
performed at the [Open Science Codefest](http://nceas.github.io/open-science-codefest/) and 
at the [NSF DataViz Hackathon for Polar CyberInfrastructure]
(http://nsf-polar-cyberinfrastructure.github.io/datavis-hackathon/).

Data Format 
=========== 
Data is in the [Common Crawl Architecture](https://wiki.apache.org/nutch/CommonCrawlDataDumper)
specification, according to the Memex format.

Each dataset has an accompanying JSON file that lists the total records,
by mimeType. A program, aggregate.py, aggregates all of the JSON files.
Total records at time of generation is provided below:

``` 
Total: 1,741,530 records
{
    "application/atom+xml": "2984",
    "application/dita+xml; format=concept": "345",
    "application/epub+zip": "36",
    "application/fits": "24",
    "application/gzip": "2060",
    "application/java-vm": "1",
    "application/msword": "244",
    "application/octet-stream": "211687",
    "application/ogg": "26",
    "application/pdf": "44658",
    "application/postscript": "219",
    "application/rdf+xml": "1042",
    "application/rss+xml": "8894",
    "application/rtf": "53",
    "application/vnd.google-earth.kml+xml": "298",
    "application/vnd.ms-excel": "227",
    "application/vnd.ms-excel.sheet.4": "1",
    "application/vnd.ms-htmlhelp": "1",
    "application/vnd.oasis.opendocument.presentation": "1",
    "application/vnd.oasis.opendocument.text": "10",
    "application/vnd.rn-realmedia": "105",
    "application/vnd.sun.xml.writer": "1",
    "application/x-7z-compressed": "2",
    "application/x-bibtex-text-file": "13",
    "application/x-bittorrent": "3",
    "application/x-bzip": "6",
    "application/x-bzip2": "63",
    "application/x-compress": "44",
    "application/x-debian-package": "4",
    "application/x-elc": "324",
    "application/x-executable": "35",
    "application/x-font-ttf": "9",
    "application/x-gtar": "46",
    "application/x-hdf": "41",
    "application/x-java-jnilib": "5",
    "application/x-lha": "2",
    "application/x-matroska": "66",
    "application/x-msdownload": "72",
    "application/x-msdownload; format=pe": "1",
    "application/x-msdownload; format=pe32": "16",
    "application/x-msmetafile": "6",
    "application/x-rar-compressed": "1",
    "application/x-rpm": "3",
    "application/x-sh": "5680",
    "application/x-shockwave-flash": "141",
    "application/x-sqlite3": "1",
    "application/x-stuffit": "1",
    "application/x-tar": "37",
    "application/x-tex": "17",
    "application/x-tika-msoffice": "2809",
    "application/x-tika-ooxml": "1775",
    "application/x-xz": "11",
    "application/xhtml+xml": "385751",
    "application/xml": "21000",
    "application/xslt+xml": "7",
    "application/zip": "3762",
    "audio/basic": "54",
    "audio/mp4": "18",
    "audio/mpeg": "646",
    "audio/vorbis": "5",
    "audio/x-aiff": "10",
    "audio/x-flac": "2",
    "audio/x-mpegurl": "1",
    "audio/x-ms-wma": "55",
    "audio/x-wav": "59",
    "image/gif": "40049",
    "image/jpeg": "85879",
    "image/png": "37997",
    "image/svg+xml": "342",
    "image/tiff": "477",
    "image/vnd.adobe.photoshop": "4",
    "image/vnd.dwg": "3",
    "image/vnd.microsoft.icon": "1570",
    "image/x-bpg": "7",
    "image/x-ms-bmp": "59",
    "image/x-xcf": "1",
    "message/rfc822": "182",
    "message/x-emlx": "1",
    "text/html": "739588",
    "text/plain": "137335",
    "text/troff": "2",
    "text/x-diff": "1",
    "text/x-jsp": "3",
    "text/x-perl": "14",
    "text/x-php": "25",
    "text/x-python": "5",
    "text/x-vcard": "19",
    "video/mp4": "675",
    "video/mpeg": "255",
    "video/quicktime": "954",
    "video/x-flv": "13",
    "video/x-m4v": "203",
    "video/x-ms-asf": "26",
    "video/x-ms-wmv": "139",
    "video/x-msvideo": "96",
    "xscapplication/zip": "85"
}
```

Data Size 
========= 
This dataset consists of 158Gb of data in the [Common
Crawl Architecture](https://wiki.apache.org/nutch/CommonCrawlDataDumper)
format and 1,741,530 records.

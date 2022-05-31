# Translo Translation API

<div align="left">
<h3>Local translation API</h3>
<img src="https://i.ibb.co/bLj3PHx/ezgif-3-3ac8a3ea5713.gif" align="left"/>
If you're already connected to the https://rapidapi.com/armangokka/api/translo/, then here is how you can decrease your ping
<br/><br/><br/><br/><br/>
</div>

## Installation

To install Translo API Local, download binary executable file in folder binaries

```
$ ./transloapi
$TRANSLO_RAPIDAPI_KEY is empty
Enter your RapidAPI-Key from Translo API: 
```
Paste your X-RapidAPI-Key from https://rapidapi.com/armangokka/api/translo/
<img src="https://i.ibb.co/nwskcd6/image.png" align="right"/>

```
...
API was launched at port 8085
```

Then just change API host of your requests from "https://translo.p.rapidapi.com/" to "http://localhost:8085/". Specification is the same.
## Before:
```
curl --request GET \
	--url 'https://translo.p.rapidapi.com/api/v3/detect?text=Dick' \
	--header 'X-RapidAPI-Host: translo.p.rapidapi.com' \
	--header 'X-RapidAPI-Key: a796038a2edpkah25b9sa336f8427p16149ajsn5712a8ab89a2'
```
## After:
```
curl --request GET \
	--url 'http://localhost:8085/api/v3/detect?text=Dick' \
	--header 'X-RapidAPI-Host: translo.p.rapidapi.com' \
	--header 'X-RapidAPI-Key: a796038a2edpkah25b9sa336f8427p16149ajsn5712a8ab89a2'
```

Keep in mind that your API quota is the same as in RapidAPI. Counter of requests on the website and counter here are the same.

# Translo Translation API
<h3>Local translation API</h3>
If you're already connected to the https://rapidapi.com/armangokka/api/translo/, then here is how you can decrease your ping

# Installation

To install Translo API Local, download binary executable file in folder /binaries

| OS          | File                     |
|-------------|--------------------------|
| Linux x64   | transloapi_linux_amd64   |
| Windows X64 | transloapi_windows_amd64 |
| MacOS       | transloapi_darwin_amd64  |
| FreeBSD x64 | transloapi_freebsd_amd64 |
| NetBSD x64  | transloapi_netbsd_amd64  |
| Linux x32   | transloapi_linux_386     |
| Windows X32 | transloapi_windows_386   |

```
$ ./transloapi_linux_amd64
$TRANSLO_RAPIDAPI_KEY is empty
Enter your RapidAPI-Key from Translo API: 
```
Paste your X-RapidAPI-Key from https://rapidapi.com/armangokka/api/translo/
<img src="https://i.ibb.co/nwskcd6/image.png" align="right"/>

```
...
$PORT is empty. Set as 8085
API was launched at port 8085
```

Then just change API host of your requests from "https://translo.p.rapidapi.com/" to "http://localhost:8085/". Specification is the same.
## Before:
```
curl --request POST \
	--url https://translo.p.rapidapi.com/api/v3/translate \
	--header 'X-RapidAPI-Key: a796038a2edpkah25b9sa336f8427p16149ajsn5712a8ab89a2' \
	--data to=ru \
	--data text=Hello \
```
## After:
```
curl --request POST \
	--url http://localhost:8085/api/v3/translate \
	--header 'X-RapidAPI-Key: a796038a2edpkah25b9sa336f8427p16149ajsn5712a8ab89a2' \
	--data to=ru \
	--data text=Hello \
```

Keep in mind that your API quota is the same as in RapidAPI. Counter of requests on the website and counter here are the same.

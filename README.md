# le-wildcard-cert-google-dns

Small repository to generate wildcard certificates using LetsEncrypt, Docker and the Google Cloud DNS API

## Usage:
* Follow the steps [here](https://certbot-dns-google.readthedocs.io/en/stable/) and save the JSON credential file to `.secrets/google.json` 
* Change the domain in `./run`
* Run `./run`
* Pull your certificate from `./etc/letsencrypt/live/<domain>` and install it somewhere, pay attention, these are symbolic links so be sure to grab the actual file
* After you're done, clean this repository to remove any secret credentials:

```bash
# git clean -fdX
```

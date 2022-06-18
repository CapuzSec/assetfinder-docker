# assetfinder

Find domains and subdomains potentially related to a given domain.



## Usage

Original Repo: https://github.com/tomnomnom/assetfinder

```
git clone https://github.com/CapuzSec/assetfinder-docker.git; cd assetfinder-docker
docker build -qt assetfinder . 
docker run -t assetfider [--subs-only] <domain>
```

## Sources

Please feel free to issue pull requests with new sources! :)

### Implemented
* crt.sh
* certspotter
* hackertarget
* threatcrowd
* wayback machine
* dns.bufferover.run
* facebook
    * Needs `FB_APP_ID` and `FB_APP_SECRET` environment variables set (https://developers.facebook.com/)
    * You need to be careful with your app's rate limits
* virustotal
    * Needs `VT_API_KEY` environment variable set (https://developers.virustotal.com/reference)
* findsubdomains
    * Needs `SPYSE_API_TOKEN` environment variable set (the free version always gives the first response page, and you also get "25 unlimited requests") — (https://spyse.com/apidocs)

### Sources to be implemented
* http://api.passivetotal.org/api/docs/
* https://community.riskiq.com/ (?)
* https://riddler.io/
* http://www.dnsdb.org/
* https://certdb.com/api-documentation 

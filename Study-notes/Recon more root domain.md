Root domains are not subdomains. We can get root domains from:
https://rashahacks.com/enumerate-root-domain-names/

crt.sh
Google, or other search engines.
ASN/IP addresses, reverse IP lookup
JS files
Redirections
Shodan

crt.sh
wget https://crt.sh/?q=Paytm+Payments&output=json -O crtsh.txt ;
cat crtsh.txt | jq | grep common_name | cut -d':' -f2 | cut -d'"' -f2 | sort -u | tee -a domains.txt

Google dorking
intext:"Tesla © 2022"

ASN/IP addresses, reverse IP lookup
Use bgp.he.net to find ASNs of an organization
masscan -iL ranges.txt -p 80,443,7443,8443,8080,8081,3306 -sT

JS files
python3 LinkFinder.py -i https://redacted.com/app.js -o cli/html
Install JSMiner Extension and JSLinkFinder extensions on Burpsuite.
Go through these files once manually, I browse through all the JS files in Sublime Text Editor and my eyes always finds more endpoints and URLs then extensions and tools. Well don't look on CDN js files and libraries javascript, look for index.js, main.js,  app.js or 1.js, or 2.js like files.
Use wayback to find how these js files look in the past.

Redirections and Manual Browsing
Domain names which you are not visiting because their status code is 301 or 302 are gold mines.
Find many root domain in that and do subdomain enum for them.

Shodan
ssl:"Organization-Name"
ssl.cert.subject.cn:redacted.com
ssl.cert.issuer.cn:apple.com

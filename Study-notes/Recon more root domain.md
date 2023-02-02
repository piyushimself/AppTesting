Root domains are not subdomains. We can get root domains from:

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


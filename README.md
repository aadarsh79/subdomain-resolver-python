# Subdomain Resolver using python3
## About Subdomain Resolver v1.0

This is a python tool designed to enumerate subdomains of websites. It helps penetration testers and bug hunters collect and gather subdomains for the domain they are targeting. It enumerates subdomains using many search engines such as Google, Yahoo, Bing, Baidu and Ask. It also enumerates subdomains using Netcraft, Virustotal, ThreatCrowd, DNSdumpster and ReverseDNS.

## Installation

```
git clone https://github.com/aadarsh79/subdomain-resolver-python.git
```

## Dependencies:

Script depends on the `requests`, `dnspython` and `argparse` python modules.

- Installation on Linux
```
sudo pip install -r requirements.txt
```

## Usage:

* To list all the basic options and switches use -h switch:
```python subdomain-resolver.py -h```

* To enumerate subdomains of specific domain:
``python subdomain-resolver.py -d example.com``

* To enumerate subdomains of specific domain and show only subdomains which have open ports 80 and 443 :
``python subdomain-resolver.py -d example.com -p 80,443``

* To enumerate subdomains and use specific engines such Google, Yahoo and Virustotal engines
``python  subdomain-resolver.py -e google,yahoo,virustotal -d example.com -o output.json``

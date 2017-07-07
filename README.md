This is a CLI tool for interacting with the ipinfo.io API. Unless you purchase a 'premium' license from ipinfo.io, you will be limited to 1,000 requests per day. 

Installation: Download or clone the script, and then place it somewhere in your $PATH. 

Dependencies: Bash, curl, sed

Usage: ipinfo [IP ADDRESS]... [OPTION]...

If no IP address is provided, the public Ip of the current machine will be checked.
multiple flags are not supported by the API.

Options:
geo            -g --only-geo
city           -c --only-city
org            -o --only-org
hostname       -H --only-hostname
region         -r --only-region
country        -C --only-country
loc            -l --only-loc
help           -h --help


Examples:

myuser@my-pc:~/$ ipinfo 8.8.8.8
  ip: 8.8.8.8
  hostname: google-public-dns-a.google.com
  city: Mountain View
  region: California
  country: US
  loc: 37.3860-122.0840
  org: AS15169 Google Inc.
  postal: 94035
  phone: 650

myuser@my-pc:~$ ipinfo 8.8.8.8 -o
AS15169 Google Inc.





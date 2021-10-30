# IP-Geolocation
Takes IP address or IP addresses and runs them thru the ipgeolocation.io API to return Owner and Location

This script was created as part of the Red Siege python challenge https://redsiege.com/python

The script leverages the free API from https://api.ipgeolocation.io/. You will need to sigup for a free account to obtain an API key. You must change the <API KEY> portion of the get request in ipgeoloc.py (line 36) to your API key for the script to work. It accepts a single IP address with the -t or --target argument, a list of IPs in a text file with -f or --file argument, a single CIDR block with -c or --cidr argument, or a list of CIDR blocks with the -cf or -cfile argument. Debugging is possible with BURP or ZAp proxies using the -d or --debug argument.
  
  usage: python3 ipgeoloc.py -t 8.8.8.8
  ![image](https://user-images.githubusercontent.com/84335647/139558879-7901b957-80b8-4061-9853-cd453e7aead8.png)

  usage: python3 ipgeoloc.py -f ips.txt
  ![image](https://user-images.githubusercontent.com/84335647/139558937-bc96c0ee-cdbe-4a88-ae8d-62e31440608d.png)

  usage: python3 ipgeoloc.py -c 8.8.8.0/24
  ![image](https://user-images.githubusercontent.com/84335647/139558983-1db83285-f48f-49ec-8aa7-600e37320a96.png)

  usage: python3 ipgeoloc.py -cf cips.txt
  ![image](https://user-images.githubusercontent.com/84335647/139559083-df68b39f-7128-468b-8967-a378085b3635.png)

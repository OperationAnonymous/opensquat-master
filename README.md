Hello I am tophat Anonymous tophat I like to surf the TOR network These are my networks: 
YouTube: https://www.youtube.com/channel/UCeqcVSPaOFqXOaPenZ0kpJA 
Git Hub: https://github.com/annymousoperation 
Twitter: https://twitter.com/AnonymousOp_


How to Install
------------

```bash
    git clone https://github.com/atenreiro/opensquat
    pip install -r requirements.txt
```
Make sure you have **Python 3.6+** and **pip3** in your environment

How to Update
------------
To update your current version, just type the following commands inside the openSquat directory:
```bash
    git pull
    pip install -r requirements.txt
```
The "pip install" is just to make sure no new libs were added with the new upgrade. 


Usage Examples
------------
Edit the "keywords.txt" with your customised keywords to hunt.

```bash
    # Lazy run with default options
    python opensquat.py

    # for all the options
    python opensquat.py -h
    
    # Search for generic terms used in phishing campaigns (can lead to false positives)
    python opensquat.py -k generic.txt

    # With DNS validation (quad9)
    python opensquat.py --dns
    
    # Subdomain search
    python opensquat.py --subdomains
    
    # Check for domains with open ports 80/443
    python opensquat.py --portcheck

    # With Phishing validation (Phishing Database)
    python opensquat.py --phishing phish_results.txt

    # Save output as JSON
    python opensquat.py -o example.json -t json

    # Save output as CSV
    python opensquat.py -o example.csv -t csv

    # Conduct a certificate transparency (ct) hunt
    python opensquat.py --ct

    # Period search - registrations from the last month (default: day)
    python opensquat.py -p month

    # Tweak confidence level. The lower values bring more false positives
    # (0: very high, 1: high (default), 2: medium, 3: low, 4: very low
    python opensquat.py -c 2

    # All validations options
    python opensquat.py --phishing phishing_domains.txt --dns --ct --subdomains --portcheck 
```

To Do / Roadmap
-------------
*   ~~Integration with VirusTotal (VT) for subdomains validation~~
*   Integratration with VirusTotal (VT) for malware detection
*   ~~Use certificate transparency~~
*   ~~Homograph detection~~ done
*   ~~Improve code quality from B to A grade (codacy)~~
*   ~~PEP8 compliance~~
*   AND logical condition for keywords search (e.g: goole+login) - Thanks to Steff T.
*   Add documentation

Feature Request
-------------
To request for a new feature, create a "new issue" and describe the feature and potential use cases. If something similar already exists, you can upvote the "issue" and contribute to the discussions.

Authors
-------------
Project founder
*   OperationAnonymous [(LinkedInk)](https://github.com/OperationAnonymous)
*   Youtube [(LinkedInk)](https://www.youtube.com/channel/UCeqcVSPaOFqXOaPenZ0kpJA)

This is a fork of [phenaproxima](https://github.com/phenaproxima/DomainConstraint)'s DomainConstraint.

I'm hoping to keep it updated. As of now the only updates are bumping the dependencies up and updating the list of allowed TLDs (pulled the latest list from ICANN as of Dec 16 2019). If I get around to updating more stuff than I will contact the owner of the original repo and see if he wants to accept PRs for the updates/publish this repo to Packagist if not. Until then you can use it as a VCS repository if you need.
# DomainConstraint
A constraint for Symfony's Validator component to test if a value is a valid domain name.

The value is tested against the rules at http://en.wikipedia.org/wiki/Hostname#Restrictions_on_valid_host_names

* At least two period-delimited segments
* Cannot start or end with a period
* Each segment must be between 1 and 63 characters
* The entire thing is no greater than 255 characters
* Valid characters are 'a' to 'z', 'A' to 'Z', '0' to '9', and hyphen (-)
* Labels cannot start or end with a hyphen
* The last segment must be a support top-level domains (and there are a LOT of strange ones)

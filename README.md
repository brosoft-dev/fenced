# fenced

## What is fenced?
fenced is a _FAST_ netfilter_queue based firewall daemon designed to block _all_ traffic from a bulk set of IPs given.
The IP 'blocklists' as called within the tool can be manually defined or automatically downloaded, cached and 
periodicallly refreshed from sites such as https://www.iblocklist.com/ or as a file and referenced directly that way.

Several formats are to be supported:
* p2p blocklist
* CIDR text file
* (others pending)

Planned features:
* Inherently designed to block entire countries' IP allocation, or just allow your local
* Fast execution of thousands of rules
* Multithreaded
* Explicit top-down rule evaluation (like iptables)
* Actions on block
* File, syslog and console logging options.

## What fenced is not?
* Anything other than Layer3
* An alternative to iptables (it's more a complimentary tool)

## Why fenced?
* Viewing or managing an iptables chain with as many rules as fenced can handle isn't practical
* Mostly, I'm sick of all the botnets triggering emails/alarms/lockouts and wanted a nice solution.

## fenced uses...
* A grotesque mashup of C/C++ as my style permits.
* libcurl
* netfilter, netfilter minimal
* libconfig++

## Where's the code?

### Aug 2015
At this current stage (Aug 2015) it's pre-alpha.
Framework for the daemon, logging and some file formats are in place,
but I won't upload anything until it can run in a (very basic) functional manner.
Check back here in a month or two.

-KB

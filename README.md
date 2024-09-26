dnsspoof
========

DNS spoofer. Drops DNS responses before they hit the router then replaces them with the spoofed DNS response.

Usage
------

```shell
python dnsspoof.py -r 192.168.0.1 -v 192.168.0.5 -d domaintospoof.com
```

Spoof domaintospoof.com to point back to the attack's machine.


```shell
python dnsspoof.py -r 192.168.0.1 -v 192.168.0.5 -a -t 80.87.128.67
```

Spoof all DNS lookup requests to point to 80.87.128.67 (stallman.org). One can also use the -t option with the -d option to redirect just a specific domain to a specific IP rather than redirecting that domain to the attacker's machine.

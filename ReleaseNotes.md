Release notes for smaug 0.8.0 Beta
==========

Product: smaug - a DANE + S/MIME prototype library
Type:    Library
Version: 0.8.0 Beta
Date:    2015-03-17

Team:

* Eric Osterweil
* Glen Wiley

Purpose of this release:
=========

The software in this repository has been constructed to serve as a reference library for DANE protocols.  The
initial support is focused on S/MIME using DANE for general object level encryption and authentication.  

This prototype is tested on Red Hat Linux 6 and Mac OSX Version 10.9.

The origin of the work draws from the DANE working group in the IETF

  https://datatracker.ietf.org/wg/dane/charter/


Platforms Supported:
=========

Mac OSX 10.9
CentOS/Red Hat Linux 6.x


Known dependencies of this release:
=========

getdns version 0.1.6 and its dependencies (optional)

or 

libunbound (and its dependencies)

openssl-1.0.1j



SMIMEA Features Supported:
========

The following outlines the current status of the implementation for the smaug beta 0.8.0
per the DANE SMIMEA draft.

Certificate Discovery
------

```
<SHA224(local part)>._smimecert.<mail domain>
```

The Certificate Usage Field
------

0 or PKIX-CA -- TODO

1 or PKIX-EE -- TODO

2 or DANE-TA -- TODO

3 or DANE-EE -- Implemented


The Selector Field
------

0 or CERT --  Implemented

1 or SPKI -- Implemented

The Matching Type Field
------

0 or Full --  Implemented

1 or SHA2-256 -- Implemented

2 or SHA2-512 -- Implemented



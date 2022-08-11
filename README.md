Beneficiary Module Mobilities API
=================================

* [What is the status of this document?][statuses]
* [See the index of all other EWP Specifications][develhub]

Summary
-------

**NOTE: This is an unstable version.
If you decide to implement the client side of this API, be aware,
that until a stable version is released, this API can change to a large extent.**

It allows external clients to report their mobilities to the Beneficiary Module.

Beneficiary Module is the system for the management of projects that received
an EU grant under the Erasmus+ programme. The Tool is developed by the European Commission
for beneficiaries of these projects. In the Beneficiary Module you can provide all the information
on projects, identify participants and mobility activities, complete and update budget information,
generate and follow-up participant reports and generate and submit own report(s) to your National Agency.
The Beneficiary Module Guide can be found here: [https://wikis.ec.europa.eu/x/KKT-AQ](https://wikis.ec.europa.eu/x/KKT-AQ).


Security
--------

This version of this API uses [standard EWP Authentication and Security, Version 2][sec-v2].
Server implementers choose which security methods they
support by declaring them in their Manifest API entry.

This API handles data which is considered private. Server implementers are
allowed to forbid less-secure methods of authentication and encryption for this
API (by dropping support for them). Currently, we leave it for the server
implementers to decide which methods are "secure enough". These recommendations
MAY change in the future.


Endpoints to be implemented
---------------------------

Server implementers MUST:

 * Implement the [`report` endpoint](endpoints/report.md).
 * Implement the [`status` endpoint](endpoints/status.md).
 * Put the URLs of these endpoints in their [manifest file][discovery-api], as
   described in [manifest-entry.xsd](manifest-entry.xsd).

The details of each of these endpoints are described on separate pages of this
API specification (use the links above).


[develhub]: http://developers.erasmuswithoutpaper.eu/
[discovery-api]: https://github.com/erasmus-without-paper/ewp-specs-api-discovery
[sec-v2]: https://github.com/erasmus-without-paper/ewp-specs-sec-intro/tree/stable-v2
[statuses]: https://github.com/erasmus-without-paper/ewp-specs-management#statuses
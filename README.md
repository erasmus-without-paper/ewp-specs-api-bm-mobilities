Beneficiary Module Mobilities API
=================================

* [What is the status of this document?][statuses]
* [See the index of all other EWP Specifications][develhub]

Summary
-------

**NOTE: This is an unstable version.
If you decide to implement the client side of this API, be aware,
that until a stable version is released, this API can change to a large extent.**

The Beneficiary Module is an online tool for Higher Education Institutions (and other organisations)
to manage their project information, applications, institutional profile, encoding activities and participants,
request individual participants’ report and submit final reports to their National Agencies
for Erasmus+ (and European Solidarity Corps) projects.

The Beneficiary Module (BM) is designed, developed and maintained by the European Commission
and is being used by the so called beneficiary organisations (such as a HEI)
and National Agencies that are involved in decentralised projects.

The aim of this API is to provide a solution for HEIs that are participating in Erasmus+ KA1 mobility
of higher education individuals projects, to link their mobility management software (any type)
to the Beneficiary Module, therefore automatise reporting of individual mobility of students in the Beneficiary Module.

Only student mobility reporting is covered by this API. Staff mobility reporting may be added in the future.


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
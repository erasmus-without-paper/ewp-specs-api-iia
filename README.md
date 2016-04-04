Inter Institutional Agreement (IIA) API
======================================

* [What is the status of this document?][statuses]
* [See the index of all other EWP Specifications][develhub]

Summary
-------

This document describes the ** IIA API **. This is the API's needed to exchange interinstitutional agreements between two
or more partners. There is need for API's on both sides to be able to exchange this information.

Participants
------------

* **MASTER** - This will be the owner of the agreement. The institution that initiates the work on the agreement will be designeted
  master. The master is responsible for merging any changes that the other partners proposes to the document. This is to
  avoid the problem of different partners trying to override each other.
* **SLAVE** - The other partners in the agreement are called slaves. They cannot change the master document, only propose changes
  and accept or reject an agreement.

Basic flow
----------

Image

The Master initiates the IIA and sends the IIA-XML to all partners (slaves). The slaves can then either approve, reject or propose
changes to the IIA. This will be relayed to the master, using an XML with both structured and unstructured data (XML with text). 
Examples to come later. It is the Masters responsibility to keep track of change requests and approvals. Every time the IIA is
changed by the master (based on the change requests), the version of the IIA is changed, so the other partners can see what type
of version the document is in. There is some manual labour required by the Master, both in merging changes and keeping track of 
approvals.
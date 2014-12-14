Netconn API
+++++++++++

This repository is now frozen-in-time and will not accept new patches. To
update Networking API information, please submit patches to
http://git.openstack.org/cgit/openstack/neutron-specs for a new API feature
and to http://git.openstack.org/cgit/openstack/api-site for implemented API
information.

It was the original holder for API information for the OpenStack Networking
 project, also known as Neutron. The Neutron project provides open
source network connectivity to OpenStack Compute, the project named Nova.

Contributing
============
Our community welcomes all people interested in open source cloud computing,
and there are no formal membership requirements. The best way to join the
community is to talk with others online or at a meetup and offer contributions
through Launchpad, the OpenStack wiki, or blogs. We welcome all types of
contributions, from blueprint designs to documentation to testing to deployment
scripts.

Prerequisites
=============
`Apache Maven <http://maven.apache.org/>`_ must be installed to build the
documentation.

To install Maven 3 for Ubuntu 12.04 and later,and Debian wheezy and later::

    apt-get install maven

On Fedora 15 and later::

    yum install maven3

Building
========
To build::

    cd v2.0
    mvn clean generate-sources

The generated PDF documentation file is::

    v2.0/target/docbkx/webhelp/openstack-network/openstack-network.pdf

The root of the generated HTML documentation is::

    v2.0/target/docbkx/webhelp/openstack-network/index.html

Testing of changes and building of the manual
=============================================

Install the python tox package and run ``tox`` from the top-level
directory to use the same tests that are done as part of our Jenkins
gating jobs.

If you like to run individual tests, run:

 * ``tox -e checkniceness`` - to run the niceness tests
 * ``tox -e checksyntax`` - to run syntax checks
 * ``tox -e checkdeletions`` - to check that no deleted files are referenced
 * ``tox -e checkbuild`` - to actually build the manual

tox will use the `openstack-doc-tools package
<https://github.com/openstack/openstack-doc-tools>`_ for execution of
these tests. openstack-doc-tools has a requirement on maven for the
build check.


Installing
==========
Refer to http://docs.openstack.org to see where these documents are published
and to learn more about the OpenStack project.

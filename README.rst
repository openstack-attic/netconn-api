Netconn API
+++++++++++

This repository contains the RESTful API information for the OpenStack Network
Connectivity project, also known as Neutron. The Neutron project provides open
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

    cd netconn-api
    mvn clean generate-sources

The generated PDF documentation file is::

	netconn-api/target/docbkx/webhelp/api/openstack-network/2.0/neutron-api-guide-2.0.pdf

The root of the generated HTML documentation is::

    netconn-api/target/docbkx/webhelp/api/openstack-network/2.0/index.html

Installing
==========
Refer to http://docs.openstack.org to see where these documents are published
and to learn more about the OpenStack project.

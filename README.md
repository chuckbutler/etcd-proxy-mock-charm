# Overview

This charm is a Mock interface, strictly used in testing the ETCD Proxy
relationship. This can be depreciated once another charm is built that consumes
the ETCD proxy interface.

It was determined during development that standing up a full OpenStack deployment
to flex this relationship, was too expensive to determine that the cluster
string was present. This charm fills that void until we find another service
to replace it.

# Usage

As this charm serves no hooks, nor actual service value - this is best used with
bundletester.

    cd $CHARM
    bundletester -F -l DEBUG -v



ipee
========

Simple linux network namespace setup tool for not dealing with the lxc nightmares.

    sudo ipee ns1 10.2.11.11
    sudo ipee ns2 10.2.11.22
    sudo ipee ns3 10.2.11.33

After that, addresses listed above will be isolated in separate network namespaces ``ns1 ns2 ns3``.

(For simplicity we assume 24 bit network mask.)

For instance you can try:

    sudo ip netns exec ns1 ping 10.2.11.22

to check if it is working.


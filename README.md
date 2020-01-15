ipee
========

This is a kind of a joke project if you must really ask... <img src="https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/240/twitter/233/smiling-face-with-smiling-eyes-and-hand-covering-mouth_1f92d.png" alt="hihihi" width="69"/>

Simple linux network namespace setup tool for not dealing with the lxc nightmares.

    sudo ipee ns1 10.2.11.11
    sudo ipee ns2 10.2.11.22
    sudo ipee ns3 10.2.11.33

After that, addresses listed above will be isolated in separate network namespaces ``ns1 ns2 ns3``.

(For simplicity we assume 24 bit network mask.)

For instance you can try:

    sudo ip netns exec ns1 ping 10.2.11.22

or

    ns ns1

to check if it is working.

[//]: # ( vim:set ts=2 sw=2 et syn=markdown: )

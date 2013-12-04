cs111-lab4
==========

Did task 1 w/ forking (only downloads), started task 2

Increased the task buffer size to 2^16. The peer list was not fitting in the bounded buffer. A better solution is needed though.

Also, Ive added the following evil situations:

1)Send a very large filename to a peer - should cause them to crash.
2)Send an arbitrarily large file to a peer - should cause them to forever receive a bogus file.
3)Added "attractive" fake files to the tracker to draw in more peers.
4)In evil mode, we accept any file requests, even if we dont have the file.

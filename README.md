[![Documentation Status](https://readthedocs.org/projects/dle-encoder/badge/?version=latest)](https://dle-encoder.readthedocs.io/en/latest/?badge=latest)
[![codecov](https://codecov.io/gh/robamu-org/py-dle-encoder/branch/main/graph/badge.svg?token=GQ5VW8PKKS)](https://codecov.io/gh/robamu-org/py-dle-encoder)

DLE Encoder for Python
======

This encoder provides a simple ASCII transport layer for serial data.
A give data stream is encoded by adding a STX (0x02) char at the beginning and an ETX (0x03) char at the end.
All STX and ETX occurrences in the packet are encoded as well so the receiver can simply look for STX and ETX
occurrences to identify packets.

You can find a C++ implementation
[here](https://egit.irs.uni-stuttgart.de/fsfw/fsfw/src/branch/master/globalfunctions/DleEncoder.cpp).

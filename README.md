Sandal
======

Sandal is a model checker for fault-prone message passing systems.

Install
-------

Sandal follows Go's standard package structure. The following command will install Sandal compiler to $GOPATH/bin:

    $ go get github.com/draftcode/sandal

In addition to Sandal compiler, you need to install NuSMV to model-check a converted model that the compiler outputs.

Usage
-----

Sandal compiler converts a model written in Sandal into a NuSMV module, and write it to STDOUT. For example, the following command will convert your Sandal model to a NuSMV module and execute NuSMV:

    $ sandal your_model.sandal | nusmv

Reference
-----

Masaya Suzuki and Takuo Watanabe  
A Language Support for Exhaustive Fault-Injection in Message-Passing System Models  
1st Workshop on Logics and Model-Checking for Self-\* Systems (MOD\* 2014),  
Electronic Proceedings in Theoretical Computer Science, Vol. 68, pp. 45-58, 2014.  
http://dx.doi.org/10.4204/EPTCS.168.4


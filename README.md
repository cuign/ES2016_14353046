README
====================
Description
---------------------
The distributed operation layer (DOL) is a framework that enables the (semi-) automatic
mapping of applications onto the multiprocessor SHAPES architecture platform. The DOL
consists of basically three parts:

*DOL Application Programming Interface: The DOL defines a set of computation and
communication routines that enable the programming of distributed, parallel
applications for the SHAPES platform. Using these routines, application programmers
can write programs without having detailed knowledge about the underlying
architecture. In fact, these routines are subject to further refinement in the
hardware dependent software (HdS) layer.

*DOL Functional Simulation: To provide programmers a possibility to test their
applications, a functional simulation framework has been developed. Besides
functional verification of applications, this framework is used to obtain
performance parameters at the application level.

*DOL Mapping Optimizati on: The goal of the DOL mapping optimization is to compute
a set of optimal mappings of an application onto the SHAPES architecture platform.
In a first step, XML based specification formats have been defined that allow to
describe the application and the architecture at an abstract level. Still, all the
information necessary to obtain accurate performance estimates is contained.
How to install
---------------------

Experimental experience
---------------------

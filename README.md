# STEPCode test build repo as integrated with OpenVSP

The OpenVSP build process uses CMake's ExternalProject_Add and
GitHub Actions.  This replicates the OpenVSP structure, but for
STEPCode only.

Right now, the version of STEPCode built by OpenVSP includes
an enormous number of compiler warnings and other output that
are very distracting.  One hope for this test build is to
help clean some of that up.

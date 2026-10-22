===================================================================
 Perl 5.20.3 for Tru64 UNIX (OSF/1 5.1b) - Binary Package
 Target: alphaev56-dec-osf5.1b
===================================================================

1. DESCRIPTION
   This package contains Perl 5.20.3 built natively on Tru64 UNIX v5.1b
   (DEC Alpha EV56) using GCC 4.7.4 with 64-bit support (-Duse64bitall).
   It includes required Berkeley DB 3.1 and GDBM shared libraries:
     - libdb-3.1.so
     - libdb.so
     - libgdbm.so
     - libgdbm.so.2.0.0

2. EXTRACT & INSTALL
   Run the following commands as root to extract to /usr/local:

     # cd /usr/local
     # gzip -dc /path/to/Tru64_Perl_5.20.3_with_libs.tar.gz | /sbin/tar xvf -

3. ENVIRONMENT SETUP (.profile)
   Add the following lines to ensure /usr/local precedes the legacy system Perl:

     export PATH=/usr/local/bin:$PATH
     export LD_LIBRARY_PATH=/usr/local/lib:$LD_LIBRARY_PATH

4. VERIFICATION
   Test the installation using:

     # /usr/local/bin/perl -v
     # /usr/local/bin/perl -e 'use v5.20; say "Perl 5.20 on Tru64 works!";'
===================================================================

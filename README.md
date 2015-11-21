rhel6-python2.7-specs
=====================

Spec files for python2.7 for RHEL 6.

Building RPMs for python2.7
---------------------------
    yum -y install gcc gcc-c++ automake autoconf libtool make gdbm-devel zlib-devel bzip2-devel openssl-devel ncurses-devel sqlite-devel readline-devel tk-devel db4-devel bluez-libs-devel libtool-ltdl-devel curl-devel pcre-devel mysql-devel unzip
    yum -y install rpm-build
    python setup.py bdist_rpm --python=python2.7 --force-arch='%{_arch}'

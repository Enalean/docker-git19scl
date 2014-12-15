Build RedHat git19 software collection

How to get the packages
=======================

  $> docker build -t git19 .
  $> docker run --name=git19 git19 true
  $> docker cp git19:/home/builder/rpmbuild/RPMS $PWD
  $> docker rm git19

How to install/use the packages
===============================

  $> copy the package & setup yum repo
  $> yum install git19-git
  $> /opt/rh/git19/root/usr/bin/git --version

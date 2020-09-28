Bootstrap: shub
From: willgpaik/centos7_aci

%setup

%files

%environment
  source /opt/rh/devtoolset-8/enable
  export PATH=$PATH:/opt/sw/r/bin

%runscript

%post
  yum -y install zlib-devel bzip2-devel xz-devel pcre-devel curl-devel readline-devel
  yum -y update
  
  source /opt/rh/devtoolset-8/enable
  mkdir -p /opt/sw/r
  cd /tmp
  wget http://lib.stat.cmu.edu/R/CRAN/src/base/R-4/R-4.0.2.tar.gz
  tar -xf R-4.0.2.tar.gz
  cd R-4.0.2
  ./configure --prefix=/opt/sw/r
  make && make install
  
  cd /tmp
  rm -rf R-4.0.2*
  
  

# r_aci
Singularity recipes for R on Centos 7 for ICS ACI clusters  
If libraries are not accessible, either change the default library path (not recommended) or copy installed libraries to local directory:  
``cp -R /opt/sw/r/lib64/R/library/* /storage/home/<USER_ID>/R/x86_64-pc-linux-gnu-library/4.0/``

2019/10/22  
Base image is built with R 3.6.1

2020/9/28  
R version is updated to 4.0.2
Recipe for RStan is added

2020/9/29  
Minor fix is added to RStan recipe

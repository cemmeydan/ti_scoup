#######################################################################################
## DO NOT EDIT THIS FILE! This file was automatically generated from the dockerfile. ##
## Run dynwrap:::.container_dockerfile_to_singularityrecipe() to update this file.   ##
#######################################################################################

Bootstrap: shub

From: dynverse/dynwrap:r

%labels
    version 0.1.1

%post
    chmod -R a+r /code
    chmod a+x /code
    git clone https://github.com/hmatsu1226/SCOUP.git && cd SCOUP && make all

%files
    . /code

%runscript
    exec Rscript /code/run.R


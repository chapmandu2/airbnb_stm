ARG BASE_IMAGE=unspecified
FROM ${BASE_IMAGE}

#####################
#install linux dependencies for png package
#####################

#reporting and stminsights
RUN yum -y install libpng-devel 

####################
#install R packages
####################

#png packages
RUN R -e "install.packages(c('png'), repos='http://cran.r-project.org')"

################
# expose ports and binding context
################

# No need for EXPOSE or CMD as inherits from chs-stage-03-rstudio


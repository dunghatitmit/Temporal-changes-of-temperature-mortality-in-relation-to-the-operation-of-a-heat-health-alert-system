##################################################################################################### 
Temporal-changes-of-temperature-mortality-in-relation-to-the-operation-of-a-heat-health-alert-system
  
  January 2022
######################################################################################################

# READ DATSET

library(readstata13) 

setwd("C:/Users/uqtphung/OneDrive - The University of Queensland/UQ/Research/Publications/Victoria Study/Data/mortality") 

data<-read.dta13("vic_mortality.dta") 

# PACKAGE FOR DLNM
library(dlnm) ; library(splines) ; library(tsModel)

# CHECK VERSION OF THE PACKAGE
  if(packageVersion("dlnm")<"2.2.0")
    stop("update dlnm package to version >= 2.2.0")

########################################################################################################


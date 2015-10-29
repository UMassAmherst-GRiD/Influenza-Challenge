
# Getting the data 

```
library(cdcfluview)
setwd("[insert file path here]")
usflu<-get_flu_data("national", "ilinet", years=1997:2015)
regionflu<-get_flu_data("HHS", sub_region=1:10, "ilinet",
years=1997:2015)
write.csv(usflu,file="ILINet_US_98_15_4_3", na="")
write.csv(regionflu,file="ILINet_Regional_98_15_4_3", na="")
```

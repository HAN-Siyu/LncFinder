Additional models for other species are provided in this folder.  
  
Usage:  
  
```
load("gallus.data.RData")  
res1 <- LncFinder::lnc_finder(yourSequences, SS.features = TRUE, format = "SS", frequencies.file = Internal.gallus, svm.model = gallus.mod, parallel.cores = -1)  

load("C_elegans.data.RData")
res2 <- LncFinder::lnc_finder(yourSequences, SS.features = FALSE, format = "DNA", frequencies.file = Internal.C_elegans, svm.model = C_elegans.mod.no_ss, parallel.cores = -1)
```

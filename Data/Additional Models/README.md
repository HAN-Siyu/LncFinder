Additional models for other species are provided in this folder. 
  
One `*.RData` file may include following objects:  

`Internal.*` is the Frequency File of one species.  
`*.mod` is the SVM model trained with secondary structure-derived features.  
`*.mod.no_ss` is the SVM model trained without secondary structure-derived features.   
  
  
Usage:  
  
```
load("gallus.data.RData")  
res1 <- LncFinder::lnc_finder(yourSequences, SS.features = TRUE, format = "SS", frequencies.file = Internal.gallus, svm.model = gallus.mod, parallel.cores = -1)  

load("C_elegans.data.RData")
res2 <- LncFinder::lnc_finder(yourSequences, SS.features = FALSE, format = "DNA", frequencies.file = Internal.C_elegans, svm.model = C_elegans.mod.no_ss, parallel.cores = -1)
```

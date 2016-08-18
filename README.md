# Code_W2P2

##Loop read selected file & count complete cases
for (i in id) {
    datafr <- read.csv(files_full[[i]])
    nobs <- sum(complete.cases(datafr))

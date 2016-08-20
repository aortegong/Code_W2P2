# Code_W2P2

##Loop read selected file & count complete cases
for (i in id) {
    datafr <- read.csv(files_full[[i]])
    nobs <- sum(complete.cases(datafr))


Hi Andrea:

Your loop is attempting to write data to your data.frame incorrectly. What is the content of "i" during each iteration of your loop? Is that really what you're trying to write, or do you need to be more specific?

I'd suggest reading this tutorial: https://www.coursera.org/learn/r-programming/discussions/weeks/2/threads/7dMVst5NEeWAKgo1CAiqoQ

Quick tip: Would a counter variable that increments with each iteration of the loop allow you to write data to the vector sequentially? As in, writing to an index that does not exist yet, but that you define with the counter variable in your loop?

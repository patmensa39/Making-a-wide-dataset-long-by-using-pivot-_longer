# Making-a-wide-dataset-long-by-using-pivot_longer 
### loading the reading the dataset 
library(tidyverse)

philant <- read_csv("http://594442.youcanlearnit.net/pew.csv")

view(philant)


philant.long <- pivot_longer(pew, !religion, names_to = "Income", values_to = "Frequency")


view(philant.long)

library(tidyverse)
library(readxl)

data <- read_excel("input/data.xlsx", na='', col_types = c("guess", "guess", "numeric", "numeric", "guess", "guess", "guess", "guess"))

# Remove rows 23 and 48
clean_data <- data[-c(23, 48), ]

# Save the cleaned data as an RDS file
saveRDS(clean_data, "input/clean_data.rds")
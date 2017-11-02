# json-example
Example Code:  How to read a JSON file into a data frame


## Load Libraries

```{r}
library(jsonlite)
library(tidyverse)
```


## read data into dataframe

```{r}
mylist <-  fromJSON("data/example-data.json")

mydf <- remove_rownames(mylist$records$fields)

mydf
```
# json-example
Example Code:  How to read a JSON file into a data frame


## Load Libraries

```{r}
library(jsonlite)
library(tidyverse)
```


## read data into dataframe

```{r}
mydf <-  fromJSON("data/example-data.json")

easydf <- remove_rownames(mydf$records$fields)

easydf 
```
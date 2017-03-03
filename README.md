```r
# insert a timestamp
snippet tst
	`r paste("#", date(), "------------------------------------------------\n")`

# load the tidyverse and use the right color scheme
snippet tv
	library(tidyverse)
	theme_set(theme_bw())
	#theme_set(theme_bw(base_size=16) + theme(strip.background = element_blank()))
	
# initialize an RMarkdown document
snippet initrmd
	library(knitr)
	opts_chunk\$set(message=FALSE, warning=FALSE, eval=TRUE, echo=TRUE)

# get the length-unique of a vector
snippet lu
	length(unique($0))

# start a ggplot
snippet gg
	ggplot(${1:data}, aes(${2:aes})) + 
		geom_${3:geom}()
```

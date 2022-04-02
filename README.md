# Assignment9-Workflow-2 

the first code line is I upload the csv form into the r

and then I summary each column to check their characteristic 

finally, I use each dessert I liked as region to visulize the table

```{r setup, include=FALSE}
dessert <- read.csv("/Users/apple/Downloads/Psy 4960 seminar/VistaNiu-R-assignment/Assign9.csv")

summary(dessert$favorite.dessert)
summary(dessert$rating.of.dessert)
summary(dessert$number.of.dessert)

library(ggplot2)
ggplot(dessert, aes(number.of.dessert, rating.of.dessert, color = as.factor(favorite.dessert)))+geom_point()
```


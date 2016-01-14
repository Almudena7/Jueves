---
title: "Jueves"
author: "Almudena"
date: "January 14, 2016"
output: word_document
---

This is an R Markdown document. Markdown is a simple formatting syntax for authoring HTML, PDF, and MS Word documents. For more details on using R Markdown see <http://rmarkdown.rstudio.com>.

When you click the **Knit** button a document will be generated that includes both content as well as the output of any embedded R code chunks within the document. You can embed an R code chunk like this:

```{r}
summary(cars)
```

You can also embed plots, for example:

```{r, echo=FALSE}
plot(cars)
```

Note that the `echo = FALSE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.

Creamos una secuencia de números
numeros <- seq(1,100, by=1)
De las que cogemos dos muestras al azar (x,y)

x <- sample(numeros,50)
y <- sample(numeros,50)
Y las utilizamos para hacer una regresión

reg1 <- lm(x~y)
Y la resumimos

summary(reg1)
Y, por ultimo, representarla en una gráfica

plot(x~y)
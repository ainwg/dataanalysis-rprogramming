## About this project
Data frames are basically the data analyst's default way to interact with data. This project use R's built-in data frames. There's a lot of interesting, easy-to- access datasets built in R and R packages.

## Walkthrough

1. Open Rstudio Cloud
2. In console, install tidyverse package
   ```R
   install.packages("tidyverse")
   ```

3. Load ggplot2 and diamonds dataset
   ```R
   library(ggplot2)
   data("diamonds")
   ```

4. The dataset should now loaded on Environment pane

   ![ss2](https://github.com/ainwg/diamonds-dataframe/assets/87463461/cf0fd1a3-8500-41aa-a85b-768d6b7e98cf)

5. Add data frame to data viewer
   ```R
   View(diamonds)
   ```
   ![ss3](https://github.com/ainwg/diamonds-dataframe/assets/87463461/9bf3bbf6-0ab3-48d3-a6ab-49ea30b2fb47)

6. Use head() function to list out the first 6 rows to get a quick preview
   ```R
   head(diamonds)
   ```
   ![ss4](https://github.com/ainwg/diamonds-dataframe/assets/87463461/ba58c7ef-5303-4a43-afe2-a5874f528dcc)

7. Use str() function to get structure of data frame. This will give high-leve info such as column names and data type contained in the columns
   ```R
   str(diamonds)
   ```
   ![ss5](https://github.com/ainwg/diamonds-dataframe/assets/87463461/a5743e3b-68a4-465c-ac1d-9a6177a20532)

8. Use colnames() to list out the column names only
   ```R
   colnames(diamonds)
   ```
   ![ss6](https://github.com/ainwg/diamonds-dataframe/assets/87463461/5856cea0-b287-49b4-b5ab-1ee301078aa7)

9. Use mutate() function to make changes to data frame. First, load the tidyverse. Then use mutate() with 1st argument is the name of data frame wanted to change, 2nd argument is the name of data frame you want to create and put formula on how you want to calculate the new column
   ```R
   library(tidyverse)
   mutate(diamonds,carat_2=carat*100)
   ```
   ![ss7](https://github.com/ainwg/diamonds-dataframe/assets/87463461/245eee28-3630-44db-b31c-8584cd8e08c2)

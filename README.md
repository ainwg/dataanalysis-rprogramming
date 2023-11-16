## About this project
R is a programming language that can help in data analysis process.

### Objective
- Compare and contrast the R programming environment and the RStudio programming environment
- Describe the RStudio programming environment including its components and benefits
- Describe the R programming language and its programming environment
- Describe programming languages and appropriate use including examples
- Download and install R assets to a computer
- Open R and execute a command
- Differentiate between the R Console and R programming environments
- Execute operations in R using mathematical operators such as +, -, *, and /
- Download and use RStudio Desktop
- Demonstrate how to complete basic tasks in R

### Working with DataFrame

Data frames are basically the data analyst's default way to interact with data. This project use R's built-in data frames. There's a lot of interesting, easy-to- access datasets built in R and R packages.

1. Open Rstudio Cloud.
2. In console, install tidyverse package.
   ```R
   install.packages("tidyverse")
   ```

3. Load ggplot2 and diamonds dataset.
   ```R
   library(ggplot2)
   data("diamonds")
   ```

4. The dataset should now loaded on Environment pane.

   ![ss2](https://github.com/ainwg/diamonds-dataframe/assets/87463461/cf0fd1a3-8500-41aa-a85b-768d6b7e98cf)

5. Add data frame to data viewer.
   ```R
   View(diamonds)
   ```
   ![ss3](https://github.com/ainwg/diamonds-dataframe/assets/87463461/9bf3bbf6-0ab3-48d3-a6ab-49ea30b2fb47)

6. Use head() function to list out the first 6 rows to get a quick preview.
   ```R
   head(diamonds)
   ```
   ![ss4](https://github.com/ainwg/diamonds-dataframe/assets/87463461/ba58c7ef-5303-4a43-afe2-a5874f528dcc)

7. Use str() function to get structure of data frame. This will give high-leve info such as column names and data type contained in the columns.
   ```R
   str(diamonds)
   ```
   ![ss5](https://github.com/ainwg/diamonds-dataframe/assets/87463461/a5743e3b-68a4-465c-ac1d-9a6177a20532)

8. Use colnames() to list out the column names only.
   ```R
   colnames(diamonds)
   ```
   ![ss6](https://github.com/ainwg/diamonds-dataframe/assets/87463461/5856cea0-b287-49b4-b5ab-1ee301078aa7)

9. Use mutate() function to make changes to data frame. First, load the tidyverse. Then use mutate() with 1st argument is the name of data frame wanted to change, 2nd argument is the name of data frame you want to create and put formula on how you want to calculate the new column.
   ```R
   library(tidyverse)
   mutate(diamonds,carat_2=carat*100)
   ```
   ![ss7](https://github.com/ainwg/diamonds-dataframe/assets/87463461/245eee28-3630-44db-b31c-8584cd8e08c2)

### Cleaning up data

1. Open RStudio Cloud.
2. In console, install and load Here, Skimr and Janitor packages. These are the packages involved in cleaning process.
   ```R
   install.packages("here")
   library("here")
   install.packages("skimr")
   library("skimr")
   install.packages("janitor")
   library("janitor")
   ```
   
3. Install dplyr package to use some of the features.
   ```R
   install.packages("dplyr")
   library("dplyr")
   ```

4. Install palmerpenguin packages to use the dataset.
   ```R
   install.packages("palmerpanguins")
   library("palmerpenguins")
   ```

5. Use skim_without_charts() function to get comprehensive summary of the dataset.
   ```R
   skim_without_charts(penguins)
   ```
   ![ss1](https://github.com/ainwg/dataanalysis-rprogramming/assets/87463461/96904604-5d22-4620-9333-73d7a3bf875a)

6. Use glimpse() function to get quick overview of the dataset.
   ```R
   glimpse(penguins)
   ```
   ![ss2](https://github.com/ainwg/dataanalysis-rprogramming/assets/87463461/23c2b540-ce3c-4542-9eb3-eb959c52fd42)
   

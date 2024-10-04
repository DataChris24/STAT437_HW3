<div align=center>
<h1>STAT 437 - Homework 3</h1>

Homework assignment 3 from STAT 437 - High Dimensional Learning and Visualization taken from Washington State University's Global Campus during the Spring 2022 semester and was taught by Dr. Xiongzhi Chen.

This assignment's intended purpose was to become familiar with K-means clustering with the use of the `cluster` package and hierarchical clustering with the `ggdendro` package and a provided source file `Plotggdendro.r` (which allows for customization of the dendrogram).

I chose to create my own report style submission, rather than use the provided R markdown template to populate with my own code and answers. I also modified the `Plotggdendro.r` file to use official Washington State University colors.
</div>

## Table of Contents

- [Built With](https://github.com/DataChris24/STAT437_HW3?tab=readme-ov-file#built-with)
- [Getting Started](https://github.com/DataChris24/STAT437_HW3?tab=readme-ov-file#getting-started)
- [Usage](https://github.com/DataChris24/STAT437_HW3?tab=readme-ov-file#usage)
- [Contributing](https://github.com/DataChris24/STAT437_HW3?tab=readme-ov-file#contributing)
- [Acknowledgements](https://github.com/DataChris24/STAT437_HW3?tab=readme-ov-file#acknowledgements)

## Built With

- ![Static Badge](https://img.shields.io/badge/-4.1.1-blue?style=plastic&logo=r)


Docker compose and supporting files included for the ability to run RStudio within a web browser without having to install RStudio locally.

## Getting Started

There are two options to be able to run the attached R markdown code files. Run locally with RStudio or run with the attached Docker container definition.

### Running Locally

1. Have R and RStudio installed on your system
2. Download the `.rmd` file(s) and open with RStudio
3. Install any packages needed that aren't already installed. 
- **NOTE:** The `devtools` package requires many system packages as dependencies before successful installation. This package is used in the last code chunk of the `.rmd` file and can be removed, or you can use the Docker container defined in this repository to run the file with RStudio from a web browser.

### Running With Docker Container

#### Prerequisites

1. Install [Docker Desktop](https://www.docker.com/products/docker-desktop/).
2. Create or sign into a Docker account.

#### Installation

1. Clone the repository 

   ```
   git clone https://github.com/DataChris24/STAT437_HW3.git
   ```
2. In your terminal navigate to the root folder of the repo and run 

   ```
   docker compose up
   ```

   *Please note that building this container image can take up to 20 minutes. I have also included a prebuilt container image that I have uploaded to GitHub to speed up the build process. If using this prebuilt container, some modifications to the* `docker-compose.yaml` *file will need to be made*

3. When the container `cmimsstat437` has been started, navigate to your web browser of choice and go to<br>
   `http://localhost:8787`
   <br>**OR**<br>
   `http://your.ip.address.here:8787` <- This is used for Windows machines or if using a Mac or Linix based machine and `localhost` does not work.

4. When the webpage loads<br>
    - username = `rstuido` <br>
    - password = `Password1`

5. Once inside RStuido navigate to the `projects` folder in the `Files` pane (bottom right window)

6. Select either the `Mims_Chris_STAT_437_HW3.Rmd` file or the `stat437_HW3.Rmd` file to interact with the file and run each of the code blocks. **NOTE:* The first file mentioned is my work while the latter is the file supplied by Dr. Chen as a template.

7. Once you are done interacting with the file, close the browser and in your terminal run 
   
   ```
   docker compose down
   ```

   This will shut down and remove the Docker container.

Also, the PDF and/or HTML output(s) of these R markdown files have also been included in the repository for review without the need to run the code in RStudio or through the use of the Docker container.

## Usage

The purpose of this project is to show my ability to not only use R and the included packages but also my ability to create professional documentation using markdown. The `devtools` package allows for specific siting of packages and their version for reproducable results. 

I have included the Docker container definition files to also show my ability to create and use Docker containers for both development and production ready applications.

## Contributing

Since this is not an ongoing project, there will be no ability to contribute further to the project.

For any suggestions or corrections that need to be made, please submit an issue [here](https://github.com/DataChris24/STAT437_HW3/issues).

## Acknowledgements

I would like to thank Dr. Xiongzhi Chen for his excellence is teaching this course and guiding me and other students to a greater understanding of the R language and its packages for use in the data analytics field and application of statistical concepts. You can more information about Dr. Chen [here](https://www.math.wsu.edu/faculty/xchen/).

The book 'An Introduction of Statistical Learning: with Applications in R' by James, Gareth et al. was used as a reference for greater understanding of the topics discussed in this course.

- James G, Witten D, Hastie T, Tibshirani R. An Introduction to Statistical Learning: with Applications in R. 2nd ed. 2021. Springer; 2022.
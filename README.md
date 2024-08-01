# ANN with Iris Dataset

This repository demonstrates an Artificial Neural Network (ANN) implementation in R using the Iris dataset. 

## Prerequisites

- R (version 4.0+)
- RStudio (optional)
- R packages: `neuralnet`, `tidyverse`, `keras`, `tensorflow`

## Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/omarion3698/AnnInR.git
   ```

2. Install R and RStudio from their official websites.

3. Install required R packages:
   ```r
   install.packages(c("neuralnet", "keras", "tensorflow", "tidyverse"), dependencies = TRUE)
   library(neuralnet)
   library(tidyverse)
   library(tensorflow)
   install_tensorflow()
   ```

## Usage

1. Open the `LabWeek13` file in RStudio using [this link](https://posit.cloud/spaces/533413/content/8484000).
2. Click "Knit" to run the R Markdown file and generate the output.

## Model Configurations

- **Model 1:** 2 hidden layers (4, 2 neurons)
- **Model 2:** 3 hidden layers (8, 4, 2 neurons)
- **Model 3:** 10 hidden layers (8, 20, 6, 5, 4, 2, 1, 4, 5, 30 neurons)
- **Model 4:** 17 hidden layers (10, 20, 30, 40, 40, 20, 10, 40, 50, 10, 20, 30, 40, 40, 20, 10, 40 neurons)

## Results

| Hidden Layers | Accuracy (%) |
|---------------|--------------|
| 2             | 100          |
| 3             | 93.33        |
| 10            | 100          |
| 17            | 63.33        |

## Conclusion

Complexity doesn't always improve performance. Model 3 (10 hidden layers) achieved 100% accuracy, while Model 4 (17 hidden layers) had reduced accuracy (63.33%) and high memory usage.

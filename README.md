# Vehicle Damange Detection App

This app let's you drag and drop an image of a car and it will tell you what kind of damage it has.
The model is trained on third quarter front and rare view hence the picture should capture the third quarter front or rare view of a car. 

![app](app_screenshot.jpg)

### Model Details
1. Used ResNet50 for transfer learning
2. Model was trained on around 1700 images with 6 target classes
   1. Front Normal
   1. Front Crushed
   1. Front Breakage
   1. Rear Normal
   1. Rear Crushed
   1. Rear Breakage
9. The accuracy on the validation set was around 80%

### Dataset

The dataset used for training the Vehicle Damage Detection model is sourced from the research article:

- **Title**: [Automated Vehicle Damage Classification Using the Three-Quarter View Car Damage Dataset and Deep Learning Approaches](https://www.sciencedirect.com/science/article/pii/S2405844024100473)
- **Authors**: Donggeun Lee, Juyeob Lee, Eunil Park
- **Published by**: *Heliyon, Elsevier*

#### Dataset:
The **Three-Quarter View Car Damage Dataset (TQVCD)** used in this project is introduced in the referenced paper. This dataset emphasizes simplicity in labeling, data accessibility, and comprehensive information in the three-quarter view of vehicles. The dataset includes vehicle images with a **front or rear orientation**, categorized by damage type, and is specifically designed to enhance automated damage classification in the automotive industry.

#### Citation:
If you use this dataset, please cite the original paper as follows:

- Lee, D., Lee, J., & Park, E. (2024). Automated vehicle damage classification using the three-quarter view car damage dataset and deep learning approaches. *Heliyon*, 10(4), e34016. https://doi.org/10.1016/j.heliyon.2024.e34016

#### Access:
The dataset is freely available under a **Creative Commons License**. For more information on dataset access and terms of use, refer to the article [here](https://doi.org/10.1016/j.heliyon.2024.e34016).

> **Note**: The dataset includes diverse vehicle damage types from three-quarter view perspectives, improving both classification accuracy and accessibility in vehicle damage classification tasks.



### Set Up

1. To get started, first install the dependencies using:
    ```commandline
     pip install -r requirements.txt
    ```
   
2. Run the streamlit app:
   ```commandline
   streamlit run app.py

# Mars Soil Segmentation Neural Network  

This repository contains a neural network designed to segment Mars soil in images, identifying different types of terrain. Each image is analyzed to classify its pixels into five categories, helping to distinguish between various soil features on Mars.  

## Features  
- **Dataset Inspection**: The dataset was thoroughly inspected to remove outliers and "fake Mars pictures" (images containing aliens as a test for dataset validation).  
- **Data Augmentation**: Generated new samples using augmentations to enhance the training dataset.  
- **Model Training and Saving**: Trained the model on the preprocessed dataset and saved it for future use.  
- **Performance Evaluation**: Evaluated the model's performance on unseen data to assess accuracy and generalization.  

## Dataset Details  
- **Image Size**: 64x128 pixels  
- **Color Space**: Grayscale (1 channel)  
- **Input Shape**: `(64, 128)`  
- **File Format**: `.npz` (Numpy archive)  
- **Number of Classes**: 5  

### Class Labels  
| Label | Description   |  
|-------|---------------|  
| 0     | Background    |  
| 1     | Soil          |  
| 2     | Bedrock       |  
| 3     | Sand          |  
| 4     | Big Rock      |  

## Project Workflow  
1. **Dataset Preparation**  
   - Load and inspect the dataset.  
   - Remove outliers and invalid images ("fake Mars pictures").  
2. **Data Augmentation**  
   - Apply augmentations to create new samples for better generalization.  
3. **Model Development**  
   - Train the model using the preprocessed and augmented dataset.  
   - Save the trained model for further use.  
4. **Evaluation**  
   - Assess the model's performance on a separate validation/testing set.  

Feel free to explore the code and adapt it for your use case. Contributions are welcome!  

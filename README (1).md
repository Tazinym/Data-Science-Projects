
# Land cover prediction of Satellite Data in the Sundarbans region






## Project Desrciption and Methodology

•	Data collection: The first step involved downloading satellite images from Google cloud repository. 
•	Image pre-processing: The next step involved opening Landsat image bands using GDAL and then converting the images to matrix, clipping (fitting to same geospatial location) and then resizing to 64x64 pixels.
•	Calculate NDVI and NDVI change: Generating NDVI for each satellite image for both Landsat 8 and Landsat 7.
•	Classify NVDI change into categories: To define the range of vegetation the NDVI change was classified into 5 categories such as high increase, increase, High decrease, decrease, no change, 
•	Model creation and Testing: An LSTM model was used to predict the next images in our model. Here, the input was taken as the n-1 sequence of NDVI change matrix, and the output was mapped to be the next sequence of NDVI changes.

## Model Creation and Testing
	Splitting the data and reshaping it.

    Model Creation
    
	Model Fit and Predict

    Model Evaluation Metrics
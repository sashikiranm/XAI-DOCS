1. Navigate to http://xai.arya.ai/

2. Sign up as a new user and login

3. Click on the **My Models** option on the top right

4. Upload the the model on the **Add Model** option

5. Choose Model Type (saved model or h5 format)

6. Add the downloadable URL of the model and submit 

7. Once added successfully, the model will be listed as follows:
       

   > ​				token number - 1634#######88 (alphanumeric string)
   >
   > ​				Model URL - the-downloable-link
   > ​	
   >
   > ​				Model Type - saved model or h5 format
   >
   > ​				Launch Time - dd/mm/yyyy hh:mm:ss
   > ​	
   >
   > ​				View API - link to view details
   >
   > ​				DELETE - link to delete the added model 


## API DETAILS

###Request Field Parameters:

1. mode - either network analysis or decision analysis

2. token - alphanumeric string referring to the model ID 

3. is_multi_input - whether or not the model accepts multiple inputs(T/F)

4. model_input - model input as a list or numpy array

5. scaler - to scale the initial model weights (>0)

6. predictions - the model predicted value

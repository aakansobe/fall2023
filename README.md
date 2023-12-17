# fall2023

# Course Policies


### Project plan

The project plan should provide an overview of how your team will tackle
the final project, and consist of:

1.  A brief description of the project and its objectives
2.  A summary of the data and methods that will be used
3.  A table describing who will be responsible for which parts of the
    project
4.  A summary of anticipated results, including any expected
    difficulties that might be encountered

### Final project report

The final report will provide a written summary of your project,
including the progress you achieved since the presentation. It should
answer the following questions:

1.  What is the overall aim of the project and what specific Earth
    Observation problem is it trying to solve?



2.  What were the methods you developed and/or applied?


3.  What were your results?
<img src="Distribution_of_predicted_pixels.png"
style="width:100.0%" data-fig-align="center" />
Figure 1 is the distribution of tree species in each prediction image.
The x-axis are the all the 375 test data which the random forest classifier
was used for the prediction. While the y-axis show the prediction proportion of 
the species for each of the 36 pixels per each test data iamge. From the predictions,
We catergorized the predicted test data based on the majority of pixels in each image 
per the each species. From this categorization, a total of 26% of the 375 test images 
has majority of the piexls prediction being Albies_alba species. While the 74% of all 
the predictions had a majority of Acer_pseudoplatanus species.

<img src="Tree species distribution.png"
style="width:100.0%" data-fig-align="center" />

Figure 2 show the spatial distribution of the predicted test data in Germany
Form the figure, Abies_alba are predominantly in northern Germany, and Acer_pseudoplatanus are predominant species in southern Germany. 


<img src="Majority_species_predicted_Albers.png"
style="width:100.0%" data-fig-align="center" />
Figure 3. Random predicted image with majority species as Abies_alba species, 
Which means all the 36 pixels in the 6 x 6 image are predicted as Abies_alba species.

<img src="Majority_of_prediction_as_Acer.png"
style="width:100.0%" data-fig-align="center" />
Figure 4. Random predicted image with majority species as Acer_pseudoplatanus species, 
Which means all the 36 pixels in the 6 x 6 image are predicted as Acer_pseudoplatanus species.

<img src="Mixed_Predicted_Albers.png"
style="width:100.0%" data-fig-align="center" />
Figure 5. Random predicted image that has mixed prediction. 
The image has 31 pixels predicted as Abies_alba species and 5 piexls predicted as Acer_pseudoplatanus. Since Abies_alba species has greater proportion, the image is 
classified as Abies_alba species.

<img src="Mixed_Predicted_Acer.png"
style="width:100.0%" data-fig-align="center" />
Figure 6. Random predicted image that has mixed prediction. 
The image has 12 pixels predicted as Abies_alba species and 24 piexls predicted as Acer_pseudoplatanus. Since Acer_pseudoplatanus species has greater proportion, the image is classified as Acer_pseudoplatanus species.




4.  Did the results show that the project aim was realized? Was an Earth
    Observation limit pushed back (or potentially pushed back)? If this
    was a group project, how were the results of individual efforts
    integrated?


5.  What are potential improvements, and any next steps you plan to
    take?
Our project was organized in two phases, each with distinct objectives. 
Initially, our focus was on comprehending the Presto model from the creators 
and then leveraging it to first  generate predictions for the provided test data.
This required us to delve deep into the methods of the Presto model, understanding
its underlying mechanisms, and applying it effectively to make predictions.  
Secondly after thoroughly understanding and getting the model to generate predictions, 
we planned  to apply it to busia_cropland_binary_2020.tif dataset. The dataset, a 10-meter resolution map depicting cropland in Busia County, Kenya during the 2020-2021 growing 
season, presented an essential binary classification challenge. The binary map utilized 
a coding system where 0 denoted no cropland, and 1 indicated the presence of cropland. 
This dataset was obtained with thresholding predictions of an LSTM classifier trained on multi-spectral S2 time series.
Despite our project plans and potential of the Presto model, we encountered challenges 
in getting the model to run initially which was resolved. We also encountered challenges 
in getting it to generate predictions for more than two tree species. Hence, our predictions were limited to the test data for only two tree species, namely "Abies_alba" and "Acer_pseudoplatanus" predominantly found in Germany. This limitation prompted us to explore the adaptability and scalability of the model. Our subsequent endeavors aim to assess the model's performance when tasked with predicting more than two species, thereby broadening 
its applicability and utility.
The next steps of our project involve refining the Presto model to be able to make predictions of tree species, going beyond the initial scope of two. Furthermore, a crucial aspect of  
the project is to determine how we could adapt Presto and apply to datasets distinct such us our dataset for busia_cropland_binary_2020.tif  which is different from the ones it was originally trained on.

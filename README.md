# Agriculture Predictor
EASY WAY TO WATCH:

https://jonathanaarondev-agriculture-predictor-main-d7d3i8.streamlit.app/

OR:

Download the files and open cmd or terminal make sure that you installed pandas,openpyxl,streamlit and plotly-express if not just copy those lines: pip install pandas openpyxl pip install streamlit pip install plotly-express now you can run it just by typing this line:(make sure that you are on the right folder if not cd to right folder) streamlit run main.py

Data science perspective:

- Data based on 17 most common crops in Israel.
- Soil composition\yield.
- The information was collected from the UN website.

DF features:

Year, Crop, Location, K [Potassium], P [phosphorus], N [nitrogen], Average Humidity, Average Rainfall,Average Temperature

Data Preparation:

Handled duplicates,missing data values,missing rows,Zero variance features,Replace Nans values and Outliers Detection(IQR method).

Feature Scaling:

Most of the times, our dataset will contain features highly varying in magnitudes, units and range. But since, most of the machine learning algorithms use Eucledian distance between two data points in their computations, this is a problem.
If left alone, these algorithms only take in the magnitude of features neglecting the units. The results would vary greatly between different units, 5kg and 5000gms. The features with high magnitudes will weigh in a lot more in the distance calculations than features with low magnitudes.
To supress this effect, we need to bring all features to the same level of magnitudes. This can be acheived by scaling.

For our purpose:
Min-Max Normalization elected.
This technique re-scales a feature or observation value with distribution value between 0 and 1.

Model Selection:

RandomForestRegressor elected due to the model has an effective method for estimating missing data and maintains accuracy when a large propotion of data are missing. 



This project built for my final project presentation.


For more details about the project:
Download the pptx file above.


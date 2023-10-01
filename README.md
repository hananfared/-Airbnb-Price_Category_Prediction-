# -Airbnb-Price_Category_Prediction-

### **Define the problem:**

> This is a multimodality task which is to estimate the price of an Airbnb listing using multi class classification based on the photo and description provided.

> The price of a new listing, as well as the type of rental being promoted, is predicted using a multi-objective method.

### **What is the input?**
> The data is presented in the form of text and images , there is an image and a text summary for each listing.

>The training data comprises of an image and text summary with label values for the listing's kind and price range.

### **What is the output?**
> Type and price range are two of the model's outputs.

### **What data mining function is required?**
 
> **1-  Importing the Libraries & Loading the Data** 

> **2- Data exploration :** we used pandas profiling  and matplotlib libraries are used to plot the data.

> **3- Data Preprocessing**: In this step we need to clean the data to make it ready for any type of classification model.

>> ### **Preprocessing trial_1 :** 
>> 1.   For image preprocessing :
>>> * resize the image to be (64 * 64 * 2)

>> 2.   For Text Preprocessing :
>>> * Tokenization & converting to integer IDs
>>> * Remove any duplicates



>> ### **Preprocessing trial_2 with different approach:**
>> 1. Translate the 'summary' column to english.
>> 2. Drop any record that can't be translated to english.
>> 3. Remove images that can't be open.
>> 4. Resize the image to be (128X*128*3)

>> * Note : This trial requires TensorFlow 2.5 or higher. In addition, TensorFlow Hub and TensorFlow Text are required for the BERT model.




> ### **4- Models:**
1.   Model with Conv2d & Dropout layer
2.   Model with LSTM layer for text
3.   Model with GRU layer for text
4.   Model with Bi-directional Recurrent with LSTM layer
5.   Model with Bi-directional Recurrent with GRU layer
6.   Multi-objective learning.
7.   Model with Transfer Learning using **ResNet50V2** & **BERT** with TensorFlow.




> **5- Predict the category for test_new.csv to be sumbitted on Kaggle**

### **What could be the challenges?**


> Small image dimensions (64x64) or (128*128) may provide problems because they may not include enough detail or information to effectively anticipate pricing ranges.

> And also there are different languages that we must deal with it, and there are some languages that we cannot translate. We will talk about them in detail in the preprocessing trial_2 .

### **What is the impact?**


> On any Vacation rental platforms, In the agreement between the lessor and the lessee we may want to find answers to the following questions in near real-time:


>*   Does a given piece of information contradict the other?
*   Does a given piece of information imply the other?

> So, the impact of this solution could assist improve relationships and establish confidence with consumers renting these properties by streamlining the workflow for using Airbnb as a host.

### **What is an ideal solution?**

> Airbnb hosts aren’t likely to be hospitality industry experts. For people who want to make money from their otherwise vacant properties, trying to find the right rate to charge guests involves time, research, and risk. Among their challenges:

> If hosts price the property too high, it sits vacant. If the price is set too low, they lose money. Ai model that helps set prices for hosts seems to make sense and make it easier for hosts to rent their properties.

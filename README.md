# Celebal-Technologies-Internship-Project-Topic-Categorization-
<br>
In this project we had to Identify the topic of the given paragraph or article by picking up the keywords.<br>
For that we required a dataset which had a collection of paragraphs.<br>
Here, we used 20 Newsgroups Dataset<br>
The 20 Newsgroups data set is a collection of approximately 20,000 newsgroup documents, partitioned (nearly) evenly across 20 different newsgroups. To the best of my knowledge, it was originally collected by Ken Lang, probably for his Newsweeder: Learning to filter netnews paper, though he does not explicitly mention this collection. The 20 newsgroups collection has become a popular data set for experiments in text applications of machine learning techniques, such as text classification and text clustering.<br><br>

# How to use your own dataset 
<br>
To use your own dataset you need to specify the location of your dataset in the path_train variable. <br>

### Source file directory 
<br>
path_train = "Dataset-Path"   <br><br>

We used sklearn.datasets.load_files to load the files. <br>
Individual samples are assumed to be files stored a two levels folder structure such as the following:<br>

container_folder/  <br>
category_1_folder/  <br>
file_1.txt file_2.txt … file_42.txt  <br> <br>

category_2_folder/  <br>
file_43.txt file_44.txt …  <br><br>

The folder names are used as supervised signal label names. The individual file names are not important. <br> <br>

Also, in the data_tages change the "news" to your desired column name for example : "paragrahs/articles" <br>
data_tags = ["filename","category","news"]   <br>

Creation of the initial dataset <br>
The aim of this step is to get a dataset with the following structure: <br><br>

![image](https://user-images.githubusercontent.com/60377214/127752332-4bcee7fc-5ab5-491c-9505-23532315ef82.png)   <br><br>

Filename : File Path  <br>
Category : Label/Topic   <br>
News : Text for corresponding label  <br>


# How to test model on any random paragraph <br> <br>

Firstly, move to the last section of the code. <br>
To test on any random paragraphs just replace the the text in paragraph1 and paragraph2 variables to your desired text. <br>
Also, change the topics/labels in the actual_label list to the labels/topics of the text you replaced. <br><br>

actual_label = ['Topic 1/Label 1','Topic 2/Label 2']  <br><br>

If you want to try on more keep adding topics/labels to actual_label list and append all paragraphs to x_data variable. <br><br><br>



# paragraph_extraction
This code extracts paragraph from a given document corresponding to the keyword provided by the user

# Necessary libraries
I have used 2 libraries 
1) Rake_NLTK (Free Library)
2) Monkey Learn (Paid API)

You can download any one of this and use it. 

# Choosing between Monkey Learn and Rake_NLTK
This depends on your necessary, if you need good model and ready to spend go for Monkey Learn else Choose Rake_NLTK.
By the way you can use Monkey Learn to a limit of 300 for free and so if you need just for a small Institute project I suggest go for Monkey Learn

# About the Model
I have 5 functions in the model
<b>preprocessText</b>: This function takes filepath as input (File must be a text file) and process the data by removing all the headings and output the a data list that contains each paragraph as an element of the list.

<b>GetKeywords</b>: This function takes the processed data from the previous function as an input and outputs the list of keywords corresponding to each paragraph. This function is used to provide the user all the keywords from which the user can choose the keywords. I have used Rake_NLTK library in this function.

<b>createMasterDict</b>: This takes the data list obtained from <b>preprocessText</b> function, model (either Monkey learn or Rake_NLTK) and an API key (if you are using monkey learn put the API key you obtained by subscribing to Monkey Learn API or else leave it) and outputs a dictionary with 3 keys that are Keyword, para_id, paragraph.

<b>keywordSearch</b>: This function takes the keyword from the user and the dictionary obtained from <b>createMasterDict</b> function as an input and outputs the paragraph corresponding to the keywords provided by the user as a text file.

<b>helps</b>: This functions is to help you through the process. It prints out process to use this model.

# Adding this feature with other file formats like PDF, Docx and images that contains text
To use this model in other file formats(mentioned above) other than text file the task is to get the text out of the other file and save it into the tet format. Don't worry, I have made another repo that extracts text from the files. this is the link to it https://github.com/ppcool1163/Extract-text

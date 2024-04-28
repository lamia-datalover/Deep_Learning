This Python script uses TensorFlow, Spacy, and other libraries to perform sentiment analysis on French reviews of DisneyLand. Here is a detailed summary of what the code does:

<b>Importation and Data Preparation</b><br>

<b>Loading Data:</b> The script starts by importing a dataset of reviews from a specific URL using Pandas.<br>
<b>Filtering French Reviews:</b> It filters to retain only reviews in French and focuses on the relevant columns (reviews and stars).<br>
<b>Text Cleaning</b><br>

<b>Downloading a French Language Model with Spacy:</b> For text processing.<br>
<b>Cleaning Reviews:</b> The text of the reviews is cleaned to remove non-alphanumeric characters and superfluous spaces. The text is then processed to lemmatize the words and remove stop words using Spacy.<br>
<b>Text Processing with TensorFlow</b><br>

<b>Tokenization:</b> Uses TensorFlow's Tokenizer to convert reviews into sequences of numbers, keeping only the 1000 most frequent words.<br>
<b>Padding Sequences:</b> The sequences are normalized in length by padding.<br>
<b>Model Creation and Training</b><br>

<b>Defining the Model:</b> Constructs a sequential model with TensorFlow that includes an embedding layer, a global pooling layer, a dense layer, and an output layer.<br>
<b>Training the Model:</b> The model is trained with the prepared data, using mean squared error as the loss function and mean absolute error as a metric.<br>
<b>Evaluation and Visualization</b><br>

<b>Visualization of Training:</b> Displays the loss curves and the mean absolute error during training to assess the model's performance.<br>
<b>Saving Results</b><br>

<b>Extracting Weights:</b> The weights of the embedding layer are extracted and saved, along with the corresponding words for future use, possibly in visualizations or further analysis.<br>
<b>Using Logs</b><br>

<b>Saving Embeddings and Metadata:</b> The embedding vectors and corresponding words are written into TSV files for further exploration, possibly with tools like TensorBoard.<br>
This script is a comprehensive example of sentiment analysis from textual reviews, incorporating data cleaning, text processing, machine learning modeling, and result evaluation. It illustrates how to use advanced tools in natural language processing and machine learning to transform raw textual data into actionable insights.








<h1>Aadhar card information extraction with Named Entity Recognition or Object Detection</h1>
<h2>Problem Statement</h2>
<p>Make a system that takes an Aadhar Card as an input and returns all the info present in the Aadhar card like Aadhar Number, Name, Address, DoB, gender etc.</p>
<h2>Data Acquisition</h2>
<p>Data Acquisition for this project was the biggest hurdle as it's not easy to get people's Aadhar card. </p>
<p>So what I did went on google and searched for Aadhar card original Images and wallah. I was able to get 40 original Aadhar cards through google image search. As finding images were very time-consuming, I just sampled 40 pictures and finished the data acquisition. </p>
<h2>Main Goal of this Project</h2>
<p>This project's main goal was to make a kind of baseline system (model) that works okayish and can be later tuned with more data and more training. </p>
<h2>Different Approach</h2>
<p>There are two possible approaches to which we can choose. Either extract information by building a NER model or go with the Object detection approach. I'll give a summary of both methods.</p>
<h2>1. Extract Aadhar info through NER</h2>
<a href="https://github.com/rumankhan1/gov-id-info-extraction-with-spacy-od/blob/main/github_aadhar_extraction_ner.ipynb">[link to the notebook]</a> <br>
<h3>a. Training Data Preparation & Annotation</h3>
<p>First, I applied tesseract to get a text from the images and then later used an open-source annotator to annotate the data. Below is the link for the same.</p>
<a href="https://github.com/rumankhan1/ner-annotator">[link to the Github repo for the open-source annotation software]</a> <br>
<h3>b. Training model</h3>
<p>We'll prepare the code to train the model. We'll start by first creating a blank spacy model, build a NER pipeline, and add that to the model. We should make sure that there's no other in the pipeline like POS and others.</p>
<p>Then we'll update the model with our custom dataset. You can experiment with different iterations, drop rate, etc. </p>
<h3>c. Performance with NER</h3>
<p>Well, we had a tiny dataset, so we can't expect that outstanding performance. But the model is still doing reasonably well on detecting the Aadhar Number, Name and DOB from the Aadhar Card. We can expect a better performance from the model for sure if we train on a larger dataset. </p>
<h2>2. Extract Aadhar info through Object Detection</h2>
<p>I'm working on it and I'll update it soon</p>
<h3></h3>
<p></p>








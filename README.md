Download Link: https://assignmentchef.com/product/solved-cs60092-assignment3-text-classification-of-text-documents-ir
<br>
This assignment is on classification of text documents. It is highly recommended that you use python3 for this assignment as libraries like nltk will make many things easier (stop word removal and lemmatization). However, if you use any other language, you most probably have to design these modules yourselves which might not perform as good as nltk library in python. Also you can use packages from scipy for classification purposes.

<strong>Assumptions:</strong>Remove stop words, punctuation marks, make everything to lowercase and perform lemmatization to generate tokens from the document (use nltk library in python). Assume positional and class conditional independence of the terms in document for Naive Bayes. For vector space classifications, assume each document is represented by its normalized tf-idf vector representation. The tf-idf vector construction follows the same procedure as stated in assignment 2.

<a href="https://drive.google.com/file/d/1EgO6tS0NdtXsBTRnepfHelIDNf6u6pF-/view?usp=sharing"><strong>Find your dataset here</strong></a>

<ol>

 <li>Naive Bayes with feature selection

  <ul>

   <li>Select top x features using mutual information from both train data. Vary x in {1, 10, 100, 1000, 10000}.</li>

   <li>Using each of the above x, train a multinomial Naive Bayes on the given train data, with add-one smoothing.</li>

   <li>Using each of the above x, train a Bernoulli Naive Bayes on the given train data.</li>

   <li>Print F<sub>1 </sub>score for each of the classifier on the test data for each of the feature value.</li>

  </ul></li>

 <li>Vector space classification – Linear: Use Rocchio classifier to classify documents in the test data and print the F<sub>1 </sub> For Rocchio classifier, use the decision rule as follows. Assign d to class c iff |µ(c) − v(d)| &lt; |µ(c¯)−v(d)|−b. Vary b within the range {0, .01, .05, .1} and print F<sub>1 </sub>score for the b values.</li>

 <li>Vector space classification – Non linear: Use kNN classifier to classify documents in the test data and report F<sub>1 </sub> Vary k in {1, 10, 50}. For</li>

</ol>

1

similarity score use inner product of vector representation of two documents. Print F<sub>1 </sub>scores on test data.

<strong>Instructions for submission </strong>Submit your codes named as Rollno Taskno.py.

Your code will be executed as <em>python3 your-code.py path-data-directory output-file</em>

You should print F<sub>1 </sub>scores in space separated manner in the output file as simple text. Sample output should look like

Rest two files resembles similar structure
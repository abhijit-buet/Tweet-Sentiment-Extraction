# Tweet-Sentiment-Extraction

This challenge was launched in kaggle. The problem - there is a sentence and it's corresponding sentiment like positive, negative or neutral as input. We need to predict the part of the sentence that is responsible for that sentiment.
Example: The sentence: "My dog is amazing", Sentiment: "Positive", Key part of the Sentence = "amazing"

<h1> Proposed Method
<h6>
  
 I have trained a Pre-trained BERT model to solve this problem.
 Traditional BERT is made for question answering task, like we need to input the question and the context and the output will be the answer.
 We can model the above problem in a question - answering format,
 Sentiment = Question
 Sentence  = Context
 Key part of the sentence = Answer
 
<img src="https://github.com/abhijit-buet/Images/blob/main/Slide2.PNG" width = "512" height = "328">

I have used the BERT TOKENIZER for the tokenization task. Performed a three-fold training on the BERT model and ensembled the output.

<h1> Result
 <h6>
   
 The evaluation was done using Jaccard score. The proposed framework achieved a Jaccard score of 0.71.

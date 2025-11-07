![](https://github.com/AIVenture0/Email_summarization-with-Unsupervised-Learning/blob/master/Images/Email-summarization.png)

## What is Text Summarization?

__Text summarization__ is the process of distilling the most important information from a source (or sources) to produce an abridged version for a particular user (or users) and task (or tasks).

A module for __E-mail Summarization__ which uses clustering of skip-thought sentence embeddings.

<img src="https://miro.medium.com/max/1400/1*1Y12GxSbTW0Pf3Psh24zHw.png">

# Instructions
- The code is written in ```Python 3```.
- The module uses code of the ```Skip-Thoughts``` paper which can be found in the repo.
## How the whole thing process
- Very first it's all about email parsing i mean removing 

  - __Signatures__ (e-mail signature is a block of text that is appended to the end of an e-mail message you send)
  - __Salutation__ (e-mail salutation is a greeting, you write at the top of your email)
  
  
 Given above two steps are really complicated and it requires you a good understanding for __Regular Expression(Regex)__.
 
 
After these two initial steps we get the email body. Body is in different languages for using
- Google tranlate api convert them to one language"English".
- Perform Sent_tokenization 
- Using Skip-thought-vector record the sentence embedding of each sentence.
- With kmeans clustring clustre the embedding 
- After all that perform the Topic modelling on email data.




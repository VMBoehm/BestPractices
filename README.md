# Best Practices for using Machine Learning in Scientific Applications
Machine Learning (ML) methods bear a huge potential for scientific applications. However, like every method they come with their pitfalls and drawbacks. It is therefore desirable to agree as a scientific community on certain requirements that an ML method has to fullfill in order to be useful (and safe) for a scientific application.  
Motivated by the recently growing interest in using ML methods for scientific applications, this guide aims at defining guidelines for developing, describing and evaluating ML methods. It is meant to serve as a reference to both authors and referees.
It is work in progress and everyone working in this or related fields is invited to suggest additions and edits.


### To write a great ML for science paper, consider the following criteria:
- Reproducibility:   
  - Make your code public and provide instructions for reproducing your results.
  - Clearly describe 
    - any kind of preprocessing you apply to the data.
    - your training strategy.
    - parameter and architecture space you explored in order to find your best working model (how much fine tuning required)
- Robustness/Stability:
  - Show that the model still performs its task reliably under distributional shifts/ adversarial attacks. (= if the test data is slightly different to the training data) or argue why this is not an issue in your specific application.
- Uncertainty Estimates/ Biases:
  - Quantify the uncertainty of your model prediction. 
  - Show that your uncertainty estimates are reliable.
  - Show that your predictor is unbiased or less biased than alternative approaches.
- Why ML?
  - State clearly why you expect an ML method to perform better on this specific task than other approaches. 
  - What are the drawbacks (e.g. loss of interpretability) and advantages of the ML method?
  - Don’t just claim the advantages. Show them.
  - Comment on how flexible your model is. Does it need to be retrained for slightly different problem statements?
  - Is your work more than just a proof of concept? 
    - State how far is it from the current state of your work to application to real data?
    - Is it feasible to bridge this gap in the near future?
  - Are you using the ML method to replace something that we can already model optimally?
    - If so, state why it is still favorable to use the ML method? (a reason could be computational efficiency) 
    - Could you have used a model in a more targeted fashion? 


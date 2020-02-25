# Best Practices for using ML in Scientific Applications

Motivated by the vast amount of publications that propose ML methods for scientific applications, this guide aims at defining guidelines for developing, describing and evaluating these methods. It is meant to serve as a reference to both authors and referees.
It is work in process and suggestions/comments are welcome.

- Reproducibility:   
  - Make your code public and provide instructions for reproducing your results.
  - Clearly describe 
    - any kind of preprocessing you apply to the data.
    - your training strategy.
    - parameter and architecture space you explored in order to find your best working model (how much fine tuning required)
- Robustness/Stability:
  - Show that the model still performs its task reliably under distributional shifts. (= if the test data is slightly different to the training data) or argue why this is not an issue in your specific application.
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


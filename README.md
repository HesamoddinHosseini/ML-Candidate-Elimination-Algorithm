# ML-Candidate-Elimination-Algorithm

The candidate elimination algorithm incrementally builds the version space given a hypothesis space H and a set E of examples. The examples are added one by one; each example possibly shrinks the version space by removing the hypotheses that are inconsistent with the example. The candidate elimination algorithm does this by updating the general and specific boundary for each new example. 

*You can consider this as an extended form of Find-S algorithm.

*Consider both positive and negative examples.

*Actually, positive examples are used here as Find-S algorithm (Basically they are generalizing from the specification).

*While the negative example is specified from generalize form.


Step1: Load Data set

Step2: Initialize General Hypothesis  and Specific  Hypothesis.

Step3: For each training example  

Step4: If example is positive example  

          if attribute_value == hypothesis_value:
             Do nothing  
          else:
             replace attribute value with '?' (Basically generalizing it)
             
Step5: If example is Negative example  
          Make generalize hypothesis more specific.

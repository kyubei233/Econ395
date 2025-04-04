Our dataset only contain 10% of abuse case, so i try to do the unsampling in the code.
  data is imbalanced (~10% abuse).
  
  block duplicates abuser cases so both classes are equally represented in the training set.
  
  Prevents models from just predicting "no abuse" all the time.

  
Only use 8 variable for x, try not to use those may be correlated.

I add one part [Feature Importance Plot (Random Forest Only)] in the code show us ranking of predictors.

Last part (decission tree)

  From PDF:
  
    If:
    
    famsize ≤ 1.5 (lives alone)
    
    AND educ ≤ 14.5 (below college)
    
    AND ethanol ≤ 1.369 (relatively lower state alcohol consumption)
    
    AND age ≤ 36.5
    
    Then: class = Abuse


Other Notable stuff:

  beertax ≤ 0.994: Lower taxes linked to abuse.
  
  fathalc ≤ 0.5: Absence of family history of alcoholism slightly reduces risk.
  
  goodhealth ≤ 0.5: Poor self-reported health is a risk signal.
  
  age thresholds (e.g., ≤ 26.5, ≤ 36.5, ≤ 43.5) are used repeatedly to isolate younger high-risk groups.

# Readme
**Continual Learning from Partially-observed Multi-sensor Tasks** (submitted to ICDM main conference)

**Datasets Used**
1. Activity Recognition Dataset (Source dataset - https://github.com/titu1994/MLSTM-FCN/releases)
    * Daily and Sports Activities Data Set (DSADs) - Classification task
    * Human Activity Recognition (HAR) - Classification task
2.  Prognostics Dataset (Source dataset - https://ti.arc.nasa.gov/tech/dash/groups/pcoe/prognostic-data-repository/#turbofan)
    * Turbofan - Regression task

There are two folder

1.  Activity Recognition folder - For DSADs and HAR analysis.
2.  Prognostics folder - For Turbofan analysis.

**Approaches Considered**
    
    Task-Specific (TS)
    Common Generator (CG)
    Supermask Transfer (SMT)
    Upper Bound (UB)
    Independent Generator (IG)

**Dimensions Variability**

    Fixed Input Dimensions (FID)
    Variable Input Dimensions (VID)

**Type of Solver**

    Standard Solver (Standard_solver)
    Solver with CM (Solver_CM)

**Scenarios**
(In case of Activity Recognition Datasets (DSADs and HAR) not in Turbofan)
    
    Fixed Classes (FC)
    Incrementally Increasing Classes (ICC)
    Partial Changing Classes (PCC)
    
**Activity Recognition**

**Preprocessing**

   For DSADS and HAR, we use z-normalize each input dimension using sensor-wise mean and standard deviation from the train set.
   We consider 5 tasks arriving sequentially with each sequential task containing a small amount of labeled training data (only 5% of training instances in case of DSADS and HAR).
   
   **Dataset_type - Daily_Sport, HAR:
      Daily_Sport - Daily and Sports Activities Data Set
      HAR - Human Activity Recognition
  **Percentage_masked_sensors_during_training (VID case) - 40%







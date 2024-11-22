# Usage Guide for the IEEE Standard

## Prerequisites

To successfully use the Safety Assessment Software with the IEEE standard, please ensure the following steps are completed:

### 1. MATLAB Installation
Make sure you have MATLAB installed on your computer. You can download it from the official [MathWorks website](https://www.mathworks.com/products/matlab.html).

### 2. Required Files
Ensure the following files are in the same directory or project folder within MATLAB:
- [`SafetyAssessmentSoftware.mlapp`](AppFiles/SafetyAssessmentSoftware.mlapp)
- `UTp(tf)_new.txt`
- `ZT(UTp)_new.txt`
- `Test.txt`
- `Test2.txt`
- `Test3.txt`

### 3. Setting Up the Environment
- Launch MATLAB.
- Create a new project or working folder.
- Copy all the required files into the folder.
- Verify that MATLAB's **Current Folder** is set to the folder containing these files.

You are now ready to proceed with the steps specific to the IEEE standard.

## How to Use
### Input Data

1. **(user input)** Time-current characteristic(s) of the protective device(s). 
2. **(user input)** Geometric proportionality factor, kg.
3. **(user input)** Touch voltage proportionality factor, kt.
4. **(user input)** Step voltage proportionality factor, ks.
5. Calculation of maximum allowable voltage limits according to IEEE Std 80. **Selection by the user, Yes or No:** Use of high resistivity surface material?
6. **If yes: (user input)** resistivity, ρs, and thickness of the surface material layer, hs.
7. **(user input)** Resistance of the human body (typical value 1000 Ω).
8. **(user input)** k factor related to tolerable electric shock energy (typical values 0.116 and 0.157 As^0.5).
9. **(user input)** Maximum value of maximum grid current for the construction of the figures showing the safety performance curves. Input of the minimum value as well.

**Up to this point here: The safety performance curves can be plotted.
The above refer to a specific typical configuration.**

10. **Selection by the user** of the case to be evaluated: soil resistivity ρ (or ground resistance Rg).
11. **Selection by the user Yes or No:** Calculation of the maximum grid current IG according to IEEE Std 80?
12. If no: **(user input)** maximum grid current, IG.
13. If yes: **(user input)** symmetrical ground fault current fault current, If, division factor, Sf, and decrement factor, Df.
14. **Selection by the user Yes or No:** Calculation of the decrement factor Df according to IEEE Std 80?
15. If no: **(user input)** decrement factor, Df.
16. If yes: **(user input)** X/R ratio, fault duration, tf.

**The above refer to specific installations of the typical grounding configuration. 
There could be several of those in a system.** 


### Output Data
1. Plotting of Time-Current characteristic(s) of the protective device(s) curve.

2. Plotting of the basic safety performance curves (IG-ρtouch and IG-ρstep curves) and (IG-Rg,touch and IG-Rg,step curves). These include all relevant curves corresponding to the protective devices of the system.

3. Addition of point(s) showing the corresponding case(s) examined. The plot for each specific case include only the relevant curves corresponding to the protective devices of this case.


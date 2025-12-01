# Due to an incorrect upload format, this document cannot be displayed. Please refer to the other renewed version.

# Coding test submit
I uploaded it but the preview won't show, and there are a lot of extra things in the coding section that shouldn't be there, so please look at this two links.
# Modify version
file:///Users/gaotianyi/Downloads/Modify%20the%20precisionCT-gty.html
# Original version
file:///Users/gaotianyi/Downloads/CT-gty.html

#This code was developed in Jupyter Notebook using Anaconda, designed to fit the EOS equation to obtain parameters a, b, c, and d, and calculate the equilibrium volume where energy is minimized.
# For Task 1
The code first imports experimental data in Jupyter Notebook using pandas and numpy, then explicitly defines the state equation function. Subsequently, parameter fitting is performed using scipy.optimize, ultimately determining the crystal's equilibrium volume through the energy minimization principle.
My first challenge was that I didn't know how to use scipy.optimize for parameter fitting initially, so I searched for methods and operational steps used by others on Bilibili to learn and apply them in my test. Due to lacking experience in setting initial values, I tested different p0 (1, 5, 10) and found that all cases converged to similar results.
The objective of the second step is to determine the equilibrium volume based on the second law of thermodynamics, which states that materials reach equilibrium at the minimum energy state. Therefore, the fitted equation is used to locate the energy minimum, and the equilibrium volume V0 is calculated at this point. The fitting parameters used were the a, b,c, and d values obtained from the p0=10 parameter set.
# For Task 2
Based on task 1 and energy-volume data from eos.csv, I created a plot where I marked the equilibrium volume point V0 identified through the energy minimization principle in the graph.

# Modify the precision
In the initial fitting, I used data rounded to two decimal places, which yielded the first set of parameters (a, b, c, d) as seen in the 'CT-gty' results. Subsequently, during a check, I repeated the procedure using the complete dataset with all available decimal places. This produced the second set of parameters found in the 'Modify the precision' version, which differed significantly from the first.
The substantial discrepancy between these two results demonstrates the significant impact of numerical precision on the fitting outcome. Consequently, for all future calculations, I will maintain the maximum available precision of the data throughout the computational process, applying appropriate rounding only during the final presentation of the results.

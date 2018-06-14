
CoEPrA - Comparative Evaluation of Prediction Algorithms
http://www.coepra.org/

CoEPrA Group
http://groups.google.com/group/CoEPrA

CoEPrA 2006
Regression Task 1

Schedule
April 17, 2006 - Problem available online
June  16, 2006 - Prediction submission due
June  30, 2006 - Winners announced 

This is the first regression problem from the CoEPrA 2006 competition.

The task is to predict Prop_001 for 88 nona-peptides from
the files CoEPrA-2006_Regression_001_Prediction_Data.txt
and CoEPrA-2006_Regression_001_Prediction_Peptides.txt.

The regression model can be developed from the descriptors
provided in the file CoEPrA-2006_Regression_001_Calibration_Data.txt
or with descriptors computed by participants from the peptide sequences provided
in the file CoEPrA-2006_Regression_001_Calibration_Peptides.txt.


The predictions will be ranked after q^2,

          SUM (Prop_001_exp - Prop_001_pred)^2
q^2 = 1 - ------------------------------------
          SUM (Prop_001_exp - Prop_001_mean)^2

Each amino acid in a nona-peptide is described by 643 descriptors,
for a total of 643X9 = 5787 descriptors.

In a row of 5787 descriptors, the first 643 descriptors belong to
the first amino acid in the peptide chain, and so on.

These descriptors are taken from the literature, and represent
position-independent indices, i.e., an amino acid 'X' has the
same value for a property 'y' irrespective of its position in the
peptide chain.

No global descriptors for the entire peptide are included here
(such as volume, molecular weight, or solvent accessible surface area).

The participants can compute other descriptors based on the
sequences provided in tables CoEPrA-2006_Regression_001_Calibration_Peptides.txt
and CoEPrA-2006_Regression_001_Prediction_Peptides.txt.

For each position in a peptide, the last 20 descriptors represent
the Miyazawa-Jernigan row (column) for the corresponding amino acid.
If the CoEPrA 2006 participants intend to explore the use of other
amino acid similarity matrices, we recommend the AAindex database,
http://www.genome.jp/aaindex/, which is also the source of many
amino acid descriptors used in the present data modeling problem.


Submission instructions

The complete solution to the regression task must be
submitted by E-mail to iejmd@yahoo.com, before  16:00 GMT June  16, 2006.

Only one solution is accepted from each group.
The file(s) with the solution must contain:
- Names and addresses for all members of the group.
- A description of the modeling procedure.
- Definition and values for all new descriptors used in the final model.
- Calibration model and statistics. This includes descriptors,
descriptor selection procedures, validation procedures,
parameters of the calibration model (regression coefficients for MLR,
connection weights and network topology for artificial neural networks,
support vectors and weights for SVM regression, etc.).
- Predicted Prop_001 values for the 88 prediction peptides
in the order from the tables CoEPrA-2006_Regression_001_Prediction_Data.txt
CoEPrA-2006_Regression_001_Prediction_Peptides.txt.


FILES:

CoEPrA-2006_Regression_001_Calibration_Data.txt

The file contains the calibration dataset:
- 89 objects (nona-peptides)
- 643X9 = 5787 descriptors
- 1 property


CoEPrA-2006_Regression_001_Prediction_Data.txt

The file contains the prediction dataset:
- 88 objects (nona-peptides)
- 643X9 = 5787 descriptors
- NAN in the property column


CoEPrA-2006_Regression_001_Calibration_Peptides.txt

The file contains the calibration peptides:
- sequences for all 89 nona-peptides
- 1 property

CoEPrA-2006_Regression_001_Prediction_Peptides.txt

The file contains the prediction peptides:
- sequences for all 88 nona-peptides

############################################################
Ovidiu Ivanciuc
Sealy Center for Structural Biology and Molecular Biophysics
Department of Biochemistry and Molecular Biology
University of Texas Medical Branch
301 University Boulevard
Galveston, Texas 77555-0857
USA

URL: http://ivanciuc.org/

Email: oiivanci@utmb.edu
Email: iejmd@yahoo.com
IEJMD: http://www.biochempress.com
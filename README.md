# Parkinson-Prediciton
Parkinson's disease is a chronic condition that leads to the gradual loss of dopaminergic neurons in the brain. 
Studies suggest that vocal impairment is a common symptom in 70% to 90% of Parkinson's patients. 
To differentiate between healthy and Parkinson's patients, a dataset was collected consisting of biomedical voice measurements from 31 individuals, 23 of whom have Parkinson's disease. 
The "status" column is used to indicate whether an individual is healthy (assigned 0) or has Parkinson's disease (assigned 1).

Initially in ASCII CSV format, the data was converted to .xlsx for analysis. 
Attirbutes Information:

Name - ASCII subject name and recording number

MDVP:Fo(Hz) - Average vocal fundamental frequency

MDVP:Fhi(Hz) - Maximum vocal fundamental frequency

MDVP:Flo(Hz) - Minimum vocal fundamental frequency

MDVP:Jitter(%),MDVP:Jitter(Abs),MDVP:RAP,MDVP:PPQ,Jitter:DDP - Several measures of variation in fundamental frequency

MDVP:Shimmer,MDVP:Shimmer(dB),Shimmer:APQ3,Shimmer:APQ5,MDVP:APQ,Shimmer:DDA - Several measures of variation in amplitude

NHR,HNR - Two measures of ratio of noise to tonal components in the voice

status - Health status of the subject (one) - Parkinson's, (zero) - healthy

RPDE,D2 - Two nonlinear dynamical complexity measures

DFA - Signal fractal scaling exponent

spread1,spread2,PPE - Three nonlinear measures of fundamental frequency variation


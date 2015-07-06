# NonCvxMatrixCompletion

## This repository contains the following files:

###1)Demo.m : This is the demo file provided by author which has been modified such that it gives runs both the author's as well as our code on 50x60 input matrix X with 40% sampling and p=0.1 .

###2)IHT_MC.m :It optimizes following problem :min rank(X) subject to ||y - M(X)||_2<err via Iterated Hard Thresholding .

###3)IST_MC.m :It optimizes following problem :min nuclear-norm(X) subject to ||y - M(X)||_2<err via Iterated Soft Thresholding .

###4)NonCVX_MC.m :Author's code for the following :min ||S||_p subject to ||y - M(X)||_2<err, where S = svd(X) via Iterated Soft Thresholding 

###5)NonCVX_MC_replica_version.m :Author's code with the suggested changes which we modified to match with the algorithm mentioned in paper (Suggested Changes are marked by comments).

###6)X.mat : A 50x60 matrix of rank 5 used as input.

###7)IDX.dat : Random sample points used to produce Masking operator for given input matrix X (40% sampling).

## Dependencies/Requirements to run the files:

#1)Sparco since the masking operator has been defined in according to the Sparco framework. 
http://www.cs.ubc.ca/labs/scl/sparco/

#2)For comparing the results with other algorithms download the Singular Value Thresholding toolbox 
http://svt.caltech.edu/
# 560-ProjectTwo
Project two for TBANLT 560 Data Mining
End to End  Data Mining Project

Description.

This project involves generating several classification models for the same data set and then combining the output from the models in an ensemble fashion. 


The data set chosen for this Project is the "BreastCancer" data from the Mlbench library in R. For more information about mlbench, and to find extended documentation, follow this link:  https://cran.r-project.org/web/packages/mlbench/mlbench.pdf

Below is a condensed description of our data:

Description:

The objective is to identify each of a number of benign or malignant classes.  Samples arrive periodically as Dr. Wolberg reports his clinical cases. The database therefore reflects this chronological grouping of the data. This grouping information appears immediately below, having been removed from the data itself.  Each variable except for the first was converted into 11 primitive numerical attributes with values ranging from 0 through 10.  There are 16 missing attribute values.  See cited below for more details.

Usage

data(BreastCancer)

Format:
A data frame with 699 observations on 11 variables, one being a character variable, 9 being orderedor nominal, and 1 target class.

[,1]IdSample code number

[,2]Cl.thicknessClump Thickness

[,3]Cell.sizeUniformity of Cell Size

[,4]Cell.shapeUniformity of Cell Shape

[,5]Marg.adhesionMarginal Adhesion

[,6]Epith.c.sizeSingle Epithelial Cell Size

[,7]Bare.nucleiBare Nuclei

[,8]Bl.cromatinBland Chromatin

[,9]Normal.nucleoliNormal Nucleoli

[,10]MitosesMitoses

[,11]ClassClassSource


.  Creator:  Dr.  WIlliam H. Wolberg (physician); University of Wisconsin Hospital ;Madison;Wisconsin; USA

.  Donor: Olvi Mangasarian (mangasarian@cs.wisc.edu)

.  Received: David W. Aha (aha@cs.jhu.edu)


_Explanation of RMD_
This RMD takes a data set and runs it through seven different classifier models, getting outputs for each model, than creating an ensemble model with all the results. 
To get this script to work with your data you need to keep two things in mind:

1. Standardize your labels and features-  Each model will want your label to be the first column in your dataset.  This has been done in the Import Data chunk of the code.
2.  Calculation for ensemble models requires the labels to be changed from character factors to integers.  This was not done in our first step as leaving the data as it leads to easier interpretation of our classification results.  

Within each code chunk are comments describing the actions different code are taking.  Following through the document you should be able to understand the flow of data and the decision-making process of its writer. 
Below is a high level overview of the RMD file:
Our first six code chunks deal with the loading in, cleaning, splitting data into training and validation sets, and the creation of our data frame to hold all of our predictive results. 
Further code chunks all deal with a different classification model.  Pay attention to neural networks, as it is the only classifier that extends beyond a single code chunk.  
Our last code chunk combines all our models scores to find a consensus classification for each record.  The Accuracy of our ensemble model is also added to our accuracy data frame.  

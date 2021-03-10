# 560-ProjectTwo
Project two for TBANLT 560 Data Mining

Description.
This project involves generating several classification models for the same data set and then combining the output from the models in an ensemble fashion. 
An r file is provided that generates classification models using the Iris data set.  You will want to adapt this for the BreastCancer data set which is provided.  You will want to add code that combines the output from the different models using Majority rule ensemble approach.

A data mining Portfolio
Taking a portfolio approach to your data mining projects can provide you with evidence of your data mining abilities and of the types of work you can conduct.  This can be valuable for providing information about your technical abilities, your ability to conduct data analytics, and conduct data mining activities.  From an employment perspective it can help employers quickly identify who can do the necessary work.    This is particularly useful when your data mining projects look like the types of work you would do when hired.   With data mining this can be achieved by developing a portfolio of projects. The more realistic the projects are the more assurance you provide  that you will be an asset to an organization.

End to End  Data Mining Project
The  exploratory data cleaning and analysis project provide information about how well you can extract insights and present them to others. However, they don’t demonstrate that you can build systems that are customer-facing.  Ultimately, that is the target of the data mining models being developed – deployment for use.   Customer-facing systems involve code that can be run multiple times with different pieces of data to generate different outputs.   Possibly, downloading new data daily or hourly for subsequent use.
An end to end project takes in and processes data, then generates some output.  This involves developing data mining models using machine learning algorithms, but can also be another output,  such a database processing.
The key here is to make the system flexible enough to work with new data  and also i make the code easy to setup and run. Here are typical steps you’ll need to follow to build a good end to end project:

•	Find an interesting topic – You won’t focus on a single static dataset, so you’ll want to find a topic instead such as flights, electricity pricing, health.

•	Import and parse multiple datasets

•	Create classifications or predictions.   Determine the needed features and create training and test data.  Using that to make predictions or classifications.

•	Clean up and document your code


The data set chosen for this Project is the "BreastCancer" data from the Mlbench library in R. For more information about mlbench, and to find extended documentation, follow this link:  https://cran.r-project.org/web/packages/mlbench/mlbench.pdf

Below is a condensed description of our data:
Description
The objective is to identify each of a number of benign or malignant classes.  Samples arrive periodically as Dr. Wolberg reports his clinical cases. The database therefore reflects this chronological grouping of the data. This grouping information appears immediately below, having been removed from the data itself.  Each variable except for the first was converted into 11 primitive numerical attributes with values ranging from 0 through 10.  There are 16 missing attribute values.  See cited below for more details.

Usage
data(BreastCancer)

Format
A data frame with 699 observations on 11 variables, one being a character variable, 9 being orderedor nominal, and 1 target class.
[,1]IdSample code number\n
[,2]Cl.thicknessClump Thickness\n
[,3]Cell.sizeUniformity of Cell Size\n
[,4]Cell.shapeUniformity of Cell Shape\n
[,5]Marg.adhesionMarginal Adhesion\n
[,6]Epith.c.sizeSingle Epithelial Cell Size\n
[,7]Bare.nucleiBare Nuclei\n
[,8]Bl.cromatinBland Chromatin\n
[,9]Normal.nucleoliNormal Nucleoli\n
[,10]MitosesMitoses\n
[,11]ClassClassSource\n

.  Creator:  Dr.  WIlliam H. Wolberg (physician); University of Wisconsin Hospital ;Madison;Wisconsin; USA
.  Donor: Olvi Mangasarian (mangasarian@cs.wisc.edu)
.  Received: David W. Aha (aha@cs.jhu.edu)
This is the readme file for the final project for ESS 590F by Barrett Johnson and Madie Mamer.
We added a class to read the brem_cvm_eikonet.csv file, and calculate the velocities of the receiver pairs. 
To understand how Eikonet works, 
we refer you to the README.md, originally written by Smith et al. (2020). 

The primary difference in the original and our database.py file is the class we wrote to read a three-dimensional velocity model
(in the format of a .csv). 

The PNSN_CVM class evaluates the randomly generated points for the velocity by reading a simple .csv file where the columns are Latitude, Longitude, UTME, UTMW, Depth, P-wave velocity and S-wave velocity, for each node, or point of the 3D velocity model. 
The function eval() reads the .csv as a pandas dataframe and finds the two closest nodes and takes the average velocity between the two nearest points. 

Included is a Jupyter notebook to show how we ran it.

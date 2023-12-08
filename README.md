# Analysis-of-Energy-Consumption-of-Encryption-Algorithms
This project aims to analyze the energy efficiency of three different encryption algorithms: Advanced Encryption Standard, Data Encryption Standard and Triple Data Encryption Standard. A Raspberry Pi will be used to run the codes and measure the energy consumption. The results will be plotted as a graph. 

This repository contains the python codes for encyrption, moving files from one location to another and decryption using the 3 encryption alogithms along with a python code for No encryption which is just moving files from one location to another within the system.

The AES code encrypts and decyrpts a file using the Advanced Encryption Standards in CBC(Cipher Block Chaining) mode with PKCS7 padding. Similarly, the DES and 3DES codes encyrpt and decrypt a file using the Data Encryption Standard and Triple Data Encryption Standard respectively each with PKCS5 padding. Each code runs multiple number of encryptions to see how the energy consumed varies. The codes (including the no encryption code) also move a file from one location to another within the same system using shutil.move 

These codes should be run in a Raspberry Pi connected to an energy meter to measure the energy consumed by the Raspberry Pi during this process. Note down the readings and plot a graph between the logarithm of number of encryptions and the energy consumed for the three algorithms and compare the results with one another and the no encryption case to find which algorithm is the most energy efficient.

Moving the files from one location to another becomes more significant when it is done across different systems so that the security of each algorithm can also be tested. 

This repository was created as a requirement of CIS 542 - Digital Forensics course (fall 2023) at University of Massachusetts, Dartmouth.

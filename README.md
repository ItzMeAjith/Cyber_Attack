# Cyber_Attacks_detection
      ML based cyber attack detection 

Detection of different kind of cyber attacks in wireless sensor networks by processing Big dataset. (Total number of records = 2539738)

With the development of Internet technology, network security is under diverse threats. In particular, attackers can spread malicious to carry out attacks such as phishing and spam. The  detection of cyber attacks can find out using Machine learning algorithms.

For instance, malicious features cannot be extracted efficiently. Some existing detection methods are easy to evade by attackers. We design a malicious cyber-attacks detection model to solve these problems.


attack_cat|  count|
+--------------+-------+
|         Worms|    171|
|     Shellcode|   1511|
|       Fuzzers|  21795|
|      Analysis|   2184|
|           DoS|   5665|
|Reconnaissance|  13357|
|      Backdoor|   1983|
|      Exploits|  27599|
|  Not_Effected|1959471|
|       Generic|  25378|
+--------------+-------+



          Dataset
loading the Dataset from the UNSW-NB15.csv file loaded to the google drive and mounted. 
Grouping and aggregating on our desired columns lable and attack_cat in lable values 0 for normal and 1 for attack records.
+-----+-------+
|Label|  count|
+-----+-------+
|    1|  99643|
|    0|1959471|
+-----+-------+

          Data Pre-processing


In attack_cat column so many null values and duplicate found. ex: Backdoors and Backdoor are same. so taking them as unique and removing the spaces as well.

Data pre-processing / Data cleaning which is common for both Binary Classification and Multi class classification models and feature selection based on above correlation we have selected 24 top correlations (both +ve and -ve) as input to feature column to the Binary Classification model.

Model Building.
Refer ipython file for the implementation of various Machine Learning algorithms for both Binary Classification and Multi-class classification.

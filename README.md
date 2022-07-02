# Code-quality-
This project aims to give a special quality score to the code based on github community feedbacks and static software metrics of the code. 
The First step is harvesting data from github using the scraping script 'data_collector'. 
The features collected from each Repository are :
   - The code
   - Number of stars
   - Number of forks 
   - Number of issues opened and closed 
   - Number of bugs reported
   - Set of committed dates + message
   - Number of watchers
   - Number of pull requests
   - Number of days between the first and last commits
   - List of comments and docstrings for each file
   
 #### Static metrics are extracted after encoding the code and analysing it with Radon library.
 Metric from heuristic (Cyclomatic Metrics, Raw Metrics, Halstead Metric):
 
       - halstead_metric
       - percent_comment
       - halstead_vol : volume of the code
       - Number of operators and operands
       - cyclomatic_complexity
       - loc : number of lines 
       - Number single_comments
       - Number fo blank lines

 #### The next step is score aggregation for data labeling 'Bert File'
    
 #### Next is the construction of a neural network based on BERT and analyzing the code Comments (useful comments or not), On previously labeled data training 

# Data-Engineer-in-SQL-note
A study note regards to Datacamp data engineering in SQL

Moving and Processing Data: \
Data processing: 
converting $\textbf{Raw data}$ into meaningful information
1. optimize memory, process and network costs)
2. convert data type etc

Scheduling Data:
can apply to any task listed in data processing
1. Time scheduling (ex. automatically run at a specific time)
2. Sensor scheduling (ex. automatically run if a specific condition is met)

How Data is ingested:
1. Batches: sent by groups at a specific interval (can be scheduled when resources aren't being used)
2. Streams: sent individual records right away （if need the latest data)

Parallel Computing:

Reason:
1. mainly because of memory
2. also for processing power

How:\
split it up into several subtasks
distribute subtasks over several computers

Cloud Computing:
Servers on cloud: rented; don't need space; use just the resources we need; less latency
Multicloud:
use cloud service from different companies
AWS, Google cloud, azure

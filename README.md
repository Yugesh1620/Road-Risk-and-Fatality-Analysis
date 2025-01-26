# Road-Risk-and-Fatality-Analysis
Big Data Analytics Project, Road risk and Fatality Analysis using the FARS data https://www.nhtsa.gov/research-data/fatality-analysis-reporting-system-fars 

## Dataset Source 

```
https://www.nhtsa.gov/research-data/fatality-analysis-reporting-system-fars 
```

## Before running, please make sure to ingest the dataset to your HDFS on Dataproc

Follow these steps to properly ingest data to your Hadoop Distributed File System on NYU Dataproc

```
https://sites.google.com/nyu.edu/nyu-hpc/training-support/general-hpc-topics/hadoop-user-guide#h.mblzaebj2gac
```

## Running the project on NYU Dataproc

SSH to your NYU Dataproc account with gcloud SDK

```
gcloud compute ssh nyu-dataproc-m --project=hpc-dataproc-19b8 --zone=us-central1-f
```

**Note** : This requires SSO authentication with your NYU Net ID

Then run a jupyter notebook session

# Contributors
- Preetham Rakshith Prakash
- Riya Garg
- Yugesh Panta



```
jupyter notebook
```

Open a new terminal and create an SSH tunnel linking the jupyter notebook's session's localhost **PORT**, by changing the **PORT** below,

```
gcloud compute ssh nyu-dataproc-m --project hpc-dataproc-19b8 --zone us-central1-f -- -N -L PORT:localhost:PORT
```

Now, navigate to localhost:PORT in your browser on the local device to access the notebook session running on Dataproc, open the notebook and run your code.

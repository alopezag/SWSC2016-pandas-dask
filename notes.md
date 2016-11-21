## Setting-up

- Connect with the HPC (ssh vsc40xxx@login.hpc.ugent.be)
- Switch cluster (ml swap cluster/golett)
- Start a job for this workshop (
  + `qsub /apps/gent/tutorials/pandas_dask/job.sh` This will load the needed modules and start a jupyter notebook at port 8888
  + check the job `qstat -n` and look for the target node `node2443` were jupyter is running:

```
  master19.golett.gent.vsc: 
                                                                                  Req'd       Req'd       Elap
Job ID                  Username    Queue    Jobname          SessID  NDS   TSK   Memory      Time    S   Time
----------------------- ----------- -------- ---------------- ------ ----- ------ --------- --------- - ---------
751301.master19.golett  vsc40xxx    short    job.sh            14392     2     48 754048716  08:00:00 R  00:03:26
   node2443+node2444
  ```

- Connect to the jupyter notebook (http://hod.readthedocs.io/en/latest/Connecting_to_web_UIs.html)
  +  `ssh -L 8887:localhost:8888 node2443.golett.gent.vsc`
- git clone this repo

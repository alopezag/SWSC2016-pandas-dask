## Setting-up

- Connect with the HPC (ssh vsc40xxx@login.hpc.ugent.be)
- Switch cluster (ml swap cluster/golett)
- Start a job for this workshop (qsub /apps/gent/tutorials/pandas_dask/job.sh). This will load the needed modules and start a jupyter notebook at port 8888
- Connect to the jupyter notebook (http://hod.readthedocs.io/en/latest/Connecting_to_web_UIs.html)
  +  `ssh -L 8887:localhost:8888 node2443.golett.gent.vsc`
- git clone this repo

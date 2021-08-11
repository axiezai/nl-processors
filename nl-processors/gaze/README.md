Things to try
---

 1. 1D CNN + LSTM for classification: https://link.springer.com/article/10.3758%2Fs13428-018-1144-2
    - Dataset used and codebase: GazeCom and Nyström-Andersson (https://michaeldorr.de/smoothpursuit/)
 2. Not a DL approach, REMoDNaV: https://link.springer.com/article/10.3758/s13428-020-01428-x
    - Repo: https://github.com/psychoinformatics-de/remodnav


### In this folder:
   - `eyegaze_utils.py` - Provided by the BIDS dataset in `sourcedata/code/`, stitch eyegaze segments data back to consecutive time series for full movie. Intersegmen overlap is removed.

### Pre-Reqs (not in environment.yml):
   - To use `eyegaze_utils.py` you need to install `pymvpa2`, which requires `swig`, you can install this with `brew install swig` on mac or with `apt-get` on linux. 

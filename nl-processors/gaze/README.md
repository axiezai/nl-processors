Things to try
---

 1. 1D CNN + LSTM for classification: https://link.springer.com/article/10.3758%2Fs13428-018-1144-2
    - Dataset used and codebase: GazeCom and Nyström-Andersson (https://michaeldorr.de/smoothpursuit/)
 2. Not a DL approach, REMoDNaV: https://link.springer.com/article/10.3758/s13428-020-01428-x
    - Repo: https://github.com/psychoinformatics-de/remodnav


### In this folder:
   - `eyegaze_utils.py` - Provided by the BIDS dataset in `sourcedata/code/`, stitch eyegaze segments data back to consecutive time series for full movie. Intersegmen overlap is removed.
      - Usage (`python2.7`): 
         ```python
         import os
         from eyegaze_utils.py import movie_dataset

         # output path
         BASE_DIR = '/PATH/TO/SAVE/DESTINATION/'

         ds = movie_dataset(subj='03', base_path='/PATH/TO/BIDS/dataset/study_forrest')

         # save:
         ds.save(os.path.join(BASE_DIR, 'sub-03_ses-movie_task-movie_recording_eyegaze_physio.hdf5'))
         ```

### Pre-Reqs (not in environment.yml):
   - To use `eyegaze_utils.py` you need to install `pymvpa2`, which requires `swig`, you can install this with `brew install swig` on mac or with `apt-get` on linux. 

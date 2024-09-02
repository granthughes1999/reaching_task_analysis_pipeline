Create Conda env
- conda create --name reaching_task python=3.9
- conda activate reaching_task
- conda install numpy pandas matplotlib seaborn h5py tqdm jupyter
- pip install dlab
- pip install open-ephys-python-tools
- pip install pynwb==2.2.0


Debugging
1. if you are having issues with the nwbfile.add_trial_column() part of the code, check and make sure your using pynwb version 2.2.0
   - to check your pynwb version >> pip show pynwb
   - if its not 2.2.0 >> pip unintsall pynwb
   - then >> pip instal pynwb==2.2.0


How to use these notebooks
  1. start by using makeNWB.
       - pass in the raw neuropixel recording file

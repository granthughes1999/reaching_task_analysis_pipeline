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
       - pass in 3 files
         1.  the raw/root neuropixel recording file, after kilosort has been run on it (recording_folder = r'G:\Grant\neuropixels\kilosort_recordings\necab3_03_2024-08-29_20-54-06_002')
         2.  The _events.txt file created by the bahevaior GUI (frontCam_events_txt = r"G:\Grant\behavior_data\20240829\christielab\session004\20240829_christielab_session004_events.txt"
)
         3. the frame timestamps .txt file created by the behavior GUI (frontCam_timestamps = r"G:\Grant\behavior_data\necab3\20240829\christielab\session004\20240829_christielab_session004_frontCam_timestamps.txt")



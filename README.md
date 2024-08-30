Create Conda env
- conda create --name reaching_task python=3.9
- conda activate reaching_task
- conda install numpy pandas matplotlib seaborn h5py tqdm jupyter
- pip install dlab
- pip install open-ephys-python-tools
- pip install pynwb


How to use these notebooks
  1. start by using makeNWB.
       - pass in the raw neuropixel recording file

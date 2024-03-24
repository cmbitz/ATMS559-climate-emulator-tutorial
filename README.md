# ATMS559-climate-emulator-tutorial
A tutorial for exploring emulators of CMIP-class Earth System Models.

To read the original tutorial go to, but beware that some of the discussion was out of date with the code and figures, so it could set you off on the wrong track:

[climate_emulator_tutorial.ipynb](https://nbviewer.org/github/blutjens/climate-emulator-tutorial/blob/main/climate_emulator_tutorial.ipynb)

# Get on the NCAR Jupyter Hub. I recommend using Chrome

https://jupyterhub.hpc.ucar.edu/stable/hub/home

If it is your first time using the NCAR hub, watch my video on the class canvas website first. See https://canvas.uw.edu/courses/1723161/pages/introductory-videos

# Installation

```
I recommend putting this code either in your home or work space on NCAR's compute. For example, if you want to use your work space first go to that directory using the cd command from a terminal. If you want to use your own conda or miniconda install, skip the module load conda step.

cd /glade/work/$USER
git clone git@github.com:cmbitz/ATMS559-climate-emulator-tutorial.git

cd /glade/work/$USER/ATMS559-climate-emulator-tutorial 
module load conda 
conda create --name emcli 
conda activate 
pip install -r requirements.txt 
pip install -e . 
python -m ipykernel install --user --name=emcli 
```

# Start the notebook
Click on the notebook ATMS559-climate-emulator-tutorial.ipynb

# Reference
```
@misc{lutjens23climatetutorial,
    author = {Lütjens, Björn and Hadzic, Lea M. and Newman, Dava and Veillette, Mark},
    publisher = {AGU23 Fall Meeting},
    title={The Climate Pocket: Tutorial on Building Fast Emulators in Climate Modeling},
    year={2023},
    url={https://agu.confex.com/agu/fm23/meetingapp.cgi/Paper/1304372}
}
```

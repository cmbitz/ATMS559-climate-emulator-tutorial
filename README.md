# ATMS559-climate-emulator-tutorial
A tutorial for exploring emulators of CMIP-class Earth System Models.

To see the GitHub repository for the original tutorial go to,
[climate_emulator_tutorial](https://github.com/blutjens/climate-emulator-tutorial/)
but beware that some of the discussion was out of date with the code
and figures in the version on that repository, so it could set you off
on the wrong track. Instead, please use the notebook I've created for
you in this repository for our class that I've customized to run on
NCAR's Jupyter Hub.

# Get on the NCAR Jupyter Hub. I recommend using Chrome for your browser.

[jupyterhub.hpc.ucar.edu/stable/hub/home](https://jupyterhub.hpc.ucar.edu/stable/hub/home) 

If it is your first time using the NCAR Jupyter Hub or you want a
refersher, [watch my video on the class canvas website
first](https://canvas.uw.edu/courses/1723161/pages/introductory-videos)

# Installation

You will need to install the code from a Terminal on NCAR's system,
either Casper or Derecho. To get to a Terminal, go to the + tab at the
top of this section on Jupyter Hub desktop, then find the Terminal
icon and click it.

I recommend putting this code either in your home or work space on
NCAR's computes. For example, if you want to use your work directory
(like I do below) first go to that directory using the cd command from
the Terminal and then issue the git clone command as follows:

```
cd /glade/work/$USER
git clone https://github.com/cmbitz/ATMS559-climate-emulator-tutorial.git
```

Next you need to create an environment to run this code. If you want
to use your own conda or miniconda install, skip the module load conda
step. The conda and pip commands create the environment. You'll know
it works if at the end you see emcli in the list of environments and
if when you open a notebook on on NCAR's Juypter Hub and see the emcli
kernel as an option when you go to change the kernel. If that doesn't
happen, let Cecilia know right away. Thanks!

Be sure to be in your ATMS559-climate-emulator-tutorial directory and
be patient while you issue each command one at a time. Say "y" when
asked.

```
cd /glade/work/$USER/ATMS559-climate-emulator-tutorial 
module load conda 
conda create --name emcli 
conda activate emcli
pip install -r requirements.txt 
pip install -e . 
python -m ipykernel install --user --name=emcli
conda env list
```

# Start the notebook
Click on the notebook climate-emulator-tutorial-NCAR.ipynb from the directory tree on the left of the Hub Desktop

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

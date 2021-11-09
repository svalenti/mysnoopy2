# mysnoopy2
###########################################################################
# 
#                               mysnoopy2
#                              INSTALLATION
###########################################################################
mysnoopy2 is my version of the iraf snoopy version developed by Enrico Cappellaro


mysnoopy2  is written in python and requires the following package:

- Python 2.4  or Python 2.5 or Python 2.6, 2.7
   these modules have to be installed:
      - Scipy
	    - Pyraf
	    - pylab
      - Iraf 
	    pyfits or astropy fits


#############################################################################

To install mysnoopy2 copy the tar file 'pipeline.tar' from 
xxx pipeline.tar into your PYTHONPATH directory.
If you don't have a PYTHONPATH directory path, add it in your .bashrc or 
.tcsh

eg.  setenv PYTHONPATH /home/user/lib/python2.7/site-packages:

#########################################################################
WARNING: the PYTHONPATH directory should be not longer than 35 characters.
#########################################################################

Then, extract the files from the tarball

> cd $PYTHONPATH
> tar -xvf pipeline.tar

and run the inizialization.py using your version of python 

> cd pipeline
> python inizialization.py

You will be prompted for the path to your python executable, make sure to enter
this correctly.
inizialization.py will replace the right PYTHONPATH in all the programs, and 
the $HOME directory in the login.cl file included in the pipeline.

##########################################################################
WARNING: DON'T RUN the pipeline in the directory where you have YOUR
login.cl
If you do that and the pipeline crash you lose you login.cl
##########################################################################
 

# Team 7 Code Instructions

FILE ORGANIZATION
First, store the raw images in a folder in the same directory as the code, called 'student_test' (i.e., the path from code to first image will be '../student_test/E01/T1w_1mm.nii.gz'). Or in a separate folder, and change the directory datadir accordingly at the top of pre_process.ipynb.

REGISTRATION
Next, to perform skull-stripping and registration, run all cells in pre_process.ipynb. This will store registration results for E01-10 in the folder 'Team7' and those for E11-30 in the folder 'Eval_results_temp'.

SYNTHESIS
To evaluate the synthesis model, point datadir at the top of evalUNET.ipynb to the directory with evaluation T1w and registered T2w images('Eval_results_temp' by default). Then, execute all cells in evalUNET.ipynb, and the results will be stored in the 'Team7' folder.

The pytorch trained model weights can be found at the link here, and are also included in this folder:
https://1drv.ms/u/s!ArYrv_XjglIThpxAFLvuqE9p1sjHmA?e=JGA0MC
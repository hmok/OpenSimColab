# CAREN_OpenSim_Pipeline
## **Introduction:**

This pipeline follows these **eight steps** (refer to the following flow chart):

***STEP 1 Conversion***: Use collected data (`.c3d`) files to generate `.trc`, `.mot` and EMG (`.sto`)files

***STEP 2 Scaling***: Scale the generic model (`.osim`) to generate scaled model fot the specific subject

***STEP 3 IK***: Inverse kinematics

***STEP 4 ID***: Inverse dynamics 

***STEP 5 RRA***: Residual reduction algorithm

***STEP 6 SO***: Eventually we can do static optimization for predicting muscle forces/activations

***STEP 7,8 MA & JRA***: Analysis toos for muscle analysis and joint reaction force

We follow the process suggested by OpenSim and validate every step as we make progress.



## **Authors:**

This project is an internship task of **CAREN lab** in The University of Melbourne.

**Intern:** Sonia Song 

**Supervisor:** Hossein Mokhtarzadeh

## **Related Links:**

OpenSim:  https://github.com/opensim-org/opensim-core

Pyosim: https://github.com/pyomeca/pyosim

<!--![image of pipeline structure](https://github.com/SoniaSong826/CAREN_OpenSim_Pipeline/blob/master/images/image%20of%20pipeline%20structure.png)-->
![image of pipeline structure](https://raw.githubusercontent.com/hmok/OpenSimColab/main/OpenSim_Pipeline/images/image%20of%20pipeline%20structure.png)

## Package Requirements:

1. **ezc3d**: Easy to use C3D reader/writer for C++, Python and Matlab https://github.com/pyomeca/ezc3d
2. **pyomeca**: Python toolbox for biomechanics analysis   https://github.com/pyomeca
3. **OpenSim**: SimTK OpenSim C++ libraries and command-line applications, and Java/Python wrapping. https://github.com/opensim-org/opensim-core
4. **Pyosim**: Interface between OpenSim and the Pyomeca library. https://github.com/pyomeca/pyosim

## File Structure Requirements:
### *Input File Structure*:
<img src="https://raw.githubusercontent.com/hmok/OpenSimColab/main/OpenSim_Pipeline/images/input_structure.png" width="480">

Need to specify three input path A,B and C, and notice that:

1. The static pose c3d file is named as 'Calibration.c3d'.
2. The xml files in requirements folder must have specified names.

### *Output File Structure*:
After the successful execution, you will get the output files in the following structure:
<img src="https://raw.githubusercontent.com/hmok/OpenSimColab/main/OpenSim_Pipeline/images/output_structure.png" width="480">

## Usage:
Modify the three paths in the last code block:
```
# The first path need to be specified (PATH A):
# The top level path with all folders
test_input_dir = os.path.abspath('/content/drive/My Drive/CAREN_Pipeline/TEST/')

# The second path need to be specified (PATH B):
# The file path to find the mat file with testers' information
mat_file = loadmat(os.path.join(test_input_dir ,'matTable', 'all2SubjectData.mat'))

# The third path need to be specified (PATH C):
# The file path to find the original .osim model file to be scaled later
original_model = os.path.join(test_input_dir , 'model', 'test1.osim')
```

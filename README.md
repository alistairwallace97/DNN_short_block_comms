# Machine Learning for Communications with Short Block Lengths

This is the repository of the final year project of a EEE (electrical and electronic engineering) at Imperial College London. The main deliverables of the project are to reproduce the results of two recent papers on the subject of learned communication systems. The two papers are "An introduction to deep learning for the physical layer" by T.O'Shea and J.Hoydis, "End-to-end learning of a communication system without a channel model" by F.A.Aoudia J.Hoydis. These results of these two papers were not fully reproduced. 

For a thorough description of the project, it's aims, results and conclusions see the report which can be found at ./final_report/aw3515_final_report.pdf.

# User Guide

The implementation of all results relating to the O'Shea and Hoydis paper can be found in the *initial_dnn_comms.ipynb* notebook, all the results relating to the F.A.Aoudia J.Hoydis paper can be found in the *reinforcement_learning.ipynb* notebook.

In both notebooks all functions are defined at the top. The results in the notebook can be reproduced if all the cells up to the cell starting with "*es = EarlyStopping*". At this point all functions will have been defined, all data loaded, and models will have be initialised, although the weights not loaded. To load the weights into all models run the cell below the model fitting section containing all the "*.load_weights(*" functions. After this all the models will be intialised and all cells should be ready to run. If a graph can not be plotted due to one of the inputs not being initialised then run the loading cell above the graph.

If the model is being run on a Deep Learning AMI on AWS then uncomment the second cell but leave the third cell commented out. If the notebook is being run locally then uncomment the third cell but leave the second cell commented out.

All saved figures can be found in ./figures, there is also a seperate section for figures in the report in ./final_report/figures. This systems was used to provide some separation from the report and the code which was being regularly run to avoid accidentally overwriting key results. 



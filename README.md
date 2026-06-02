# My-Run-of-Compare-Transpiler-Settings
This is my run of the "Compare Transpiler Settings" notebook provided by IBM Quantum Compute Documentation. I mostly kept the notebook unchanged, except I made sure to include my channel when calling QiskitIBMRuntime. The HTML file mainly serves to show that I have run a circuit with different optimization levels and dynamical decoupling on a real quantum device.

What I learned:

1) How different optimization levels, added with techniques such as dynamical decoupling, can improve circuit performance on a quantum device. 


Installation & Usage: To open this up, I used Ubuntu to create a Python environment. This was done by opening Ubuntu and placing the following commands:

python3 -m venv venv 
source venv/bin/activate 
jupyter lab --no-browser --ip=0.0.0.0 --port [insert a port number] 
To run this, however, you will need to create a new runtime service.

To create a service to run on quantum hardware, be sure to implement the following code with at least this much information at the beginning of your cells: QiskitRuntimeService.save_account( channel="insert appropriate channel", token='insert API key', instance="insert CRN number", overwrite=True )

#Note: You can find the original notebook here - https://quantum.cloud.ibm.com/docs/en/guides/circuit-transpilation-settings

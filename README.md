# Heart-Rate-Detector
Metropolia University of Applied Sciences 2024 -1st year -Project
MicroPython libraries for the first year hardware project
This is an example project that can be used to install MicroPython libraries that are needed for
the first year hardware project. You can also use this as a template for your own
project.

To setup your Pico
You need to have git installed. Make sure that you have python installed and that is in the path. You can verify this in terminal
by running python --version or python3 --version. If you see python version then python is in the path.
You also need to have mpremote installed. To install mpremote:


pip install mpremote
or


python -m pip install mpremote


When the prerequisites are met then you can install the project and the libraries to your Pico.

Check out the repository and install libraries
Start a terminal, go to (use cd command) the directory where you want to copy the project to. Then run:
git clone --recurse-submodules https://gitlab.metropolia.fi/lansk/pico-test.git
Go to the pico-test directory and run:


.\install.cmd if you use Windows PowerShell or cmd


./install.sh if you use Linux, OSX or GitBash



Pull submodule updates
When a submodule is added a commit id is stored to the repository where the module is set up.
If the submodule is updated the updates aren't automatically applied to the repository. To get the
updates run:
git submodule update --recursive --remote
After this command you have the latest commit in your local copy of the submodule.
Note that if you do git diff right after update you see only one changed
line. The line shows that submodule commit id has changed.
To apply the changes to your remote you must add the changed submodule
with git add and commit. After the commit you will see a different
commit id next to the submodule when you view the remote repository in the browser.

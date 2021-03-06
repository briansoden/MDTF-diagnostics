**Description**
Include a summary of the change, and link the associated issue (if applicable).  
List any dependencies that are required for this change, including libraries and variables,  
and their metadata (units, frequencies, etc...). Be sure to separate PRs and issues for new PODs and PODs currently under development.

Associated issue # (replace this phrase and parentheses with the issue number)  

**How Has This Been Tested?**
Please describe the tests that you ran to verify your changes in enough detail that  
someone can reproduce them. Include any relevant details for your test configuration  
such as the Python version, package versions, expected POD wallclock time, and the   
operating system(s) you ran your tests on.

**Checklist:**
- [ ] I have reviewed my own code to ensure that if follows the [POD development guidelines](https://mdtf-diagnostics.readthedocs.io/en/latest/sphinx/dev_guidelines.html)
- [ ] The script are written in Python 3.6 or above (preferred; required if funded by a CPO grant), NCL, or R
- [ ] All of my scripts are in the diagnostics/ subdirectory, and include a main_driver script template html, and settings.jsonc
- [ ] The main_driver script header has all of the information in the POD documentation, excluding the "More about this diagnostic" section
- [ ] The POD directory and html template have the same short name as my POD
- [ ] The html template has a 1-paragraph synopsis of the POD and links to the main documentation
- [ ] If applicable, I've added a .yml file to src/conda, and my environment builds with conda_env_setup.sh 
- [ ] The POD scripts do not access the internet or networked resources
- [ ] I have commented the code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation in the POD's doc/ subdirectory
- [ ] I have created the directory input_data/obs_data/[pod short name]
- [ ] My code is portable; it uses [MDTF environment variables](https://mdtf-diagnostics.readthedocs.io/en/latest/sphinx/ref_envvars.html), and does not contain hard-coded file or directory paths
- [ ] I have added information about the raw data files to the documentation
- [ ] I have provided the code to generate digested data files from raw data files
- [ ] Each digested data file generated by the script contains numerical data (no figures), and is 3 GB or less in size
- [ ] The repository contains no extra test scripts or data files
- [ ] My branch is up-to-date with the NOAA-GFDL develop branch, and all merge conflicts are resolved

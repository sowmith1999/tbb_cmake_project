#### Trying out Intel OneAPI - TBB

This is just a starter repo for setting up TBB, and including it in CMakeLists.txt

Get the installer from here, `https://www.intel.com/content/www/us/en/developer/tools/oneapi/base-toolkit-download.html`

Extracts the files:
 `sh ./intel-cpp-essentials-2025.0.1.27_offline.sh --remove-extracted-files no -a --cli`

Inside the extracted files:
`./install.sh --help`
The installer keeps track of the installations, each installation is called a instance, and there is a default instance, here instance I think just means a install dir and whatever tools are already installed there.
`./install.sh -c --list-instances`
This is how you can install tbb to a dir, here example1, is the instance name, and any changes or removal we use the example1.
`./install.sh -c --instance='example1' -s --eula accept --components intel.oneapi.lin.tbb.devel --install-dir=/home/sowmithk/projects/tbb_cmake_project/intel`

refs:
`https://www.intel.com/content/www/us/en/docs/onetbb/get-started-guide/2022-0/integrate-onetbb.html`
`https://www.intel.com/content/www/us/en/docs/oneapi/installation-guide-linux/2025-0/command-line-options.html#BASE-COMMAND-LINE-OPTIONS`



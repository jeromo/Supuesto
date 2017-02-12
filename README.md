The answers to Supuestos 1-4 are in png files SupuestoX

Related to Supuesto 1, install 
    https://store.docker.com/community/images/jetbrains/teamcity-server
    https://store.docker.com/community/images/jetbrains/teamcity-agent
    http://ftp.stack.nl/pub/users/dimitri/doxygen-1.8.13.linux.bin.tar.gz in teamcity-agent instance.

Related to Supuesto 3, install
    docker pull coopermaa/buildroot_x86_64
    
"Supuesto" creates the app described in assumption 4.
It contains two git submodules, https://github.com/jeromo/SupuestoClient.git and https://github.com/jeromo/SupuestoServer.git
In order to build, it needs Qt 5.7 installed, (with build-tools like make installed)

To run the tests, go to subdirectories tests in both submodules, run make and launch ./tests
To run SupuestoServer, go to SupuestoServer/src, run make, launch Server
Server shows by console the host and port where is listening
To run SupuestoCLient, go to SupuestoClient/src, run make, launch Client with arguments host and port (from output console Server)

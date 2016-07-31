# Java

# Using PPA

    # option E for proxy
    $ sudo -E apt-add-repository ppa:webupd8team/java
    $ sudo apt-get update
    $ sudo apt-get install oracle-java8-installer

# Manually install Java8

        
        # this approach may give proxy errors
        # complete wget proxy settings before running apt-get install oracle-java8-set-default
        
        sudo echo "deb http://ppa.launchpad.net/webupd8team/java/ubuntu xenial main" | sudo tee /etc/apt/sources.list.d/webupd8team-java.list
        sudo echo "deb-src http://ppa.launchpad.net/webupd8team/java/ubuntu xenial main" | sudo tee -a /etc/apt/sources.list.d/webupd8team-java.list
        sudo -E apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys EEA14886
        sudo apt-get update
        sudo apt-get install oracle-java8-installer

        # check
        java -version

        # check compiler version
        javac -version

        # automatically accept Orcale JDK8 license
        # not required
        # echo oracle-java8-installer shared/accepted-oracle-license-v1-1 select true | sudo /usr/bin/debconf-set-selections

        # set Java env vars
        sudo apt-get install oracle-java8-set-default



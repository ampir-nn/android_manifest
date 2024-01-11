1.1 Installing Repo

# Make a directory where Repo will be stored and add it to the path
$ mkdir ~/bin
$ PATH=~/bin:$PATH

# Download Repo itself
$ curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo

# Make Repo executable
$ chmod a+x ~/bin/repo

1.2 Initializing Repo

# Create a directory for the source files
$ mkdir android
$ cd android

# Install Repo in the created directory
$ repo init -u https://github.com/khadas/android_manifest.git -b  khadas-vims-pie --git-lfs

# Let Repo take care of all the hard work
$ repo sync

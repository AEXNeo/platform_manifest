AOSP Extended NEO
===========

CAF based ROM.

Getting Started
---------------

To get started with Android, you'll need to get
familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

To initialize your local repository using the AOSP Extended NEO trees, use a command like this:

    repo init -u https://github.com/AEXNeo/platform_manifest.git -b nougat

Then to sync up:

    repo sync -c -f -jX --force-sync --no-clone-bundle --no-tags

Building the source
---------------

    $ . build/envsetup.sh
    $ lunch aosp_device-userdebug
    $ make -jX otapackage

where X is the number of jobs you would like to allocate to the build system.

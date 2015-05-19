# OpenSpliceHoudini

A Fabric Splice integration for Houdini.

Fabric Splice for Houdini allows you to make use of the Fabric Core inside of Houdini and use KL and the Fabric graph to perform computations using custom Houdini operators (SOP, OBJ, etc...).

Here is a short video showing it in action: https://vimeo.com/127362431

Build system for OSX and Linux. Fell free to contribute for the Windows build :)

For access to the Fabric 2.0 Beta, you’ll want to sign up to this group:
https://groups.google.com/forum/?hl=en#!forum/fabric-engine-beta

From there you can download Fabric 2.0 and clone/build FabricUI.

# Required applications and libraries

You will need Houdini, Fabric 2.0 and FabricUI

OpenSpliceHoudini.0.4.0 is tested using:
* Houdini 14.0.223
* FabricEngine 2.0 build "FabricEngine-pablo-Darwin-x86_64-20150514-182019"
* FabricUI commit number "d84cc214d9f0cb6cba874be427e06bb8d8c7c2c0"

I'm assuming both FabricEngine-2.0 and FabricUI are copied under a FABRIC_PARENT_DIR directory.
You will need Qt 4.8 to build FabricUI.

# Environment setup

Launch Houdini shell to get the Houdini environment (on Mac, ctrl + space > Houdini Terminal)

Then source Fabric2.0 (already done if you just build FabricUI) and SpliceHoudini environments:
* cd $FABRIC_PARENT_DIR/FabricEngine-pablo-Darwin-x86_64-20150514-182019
* source environment.sh
* cd $FABRIC_PARENT_DIR/SpliceHoudini
* source environment.sh

To build and install plugin:
* make install

To clean:
* make clean_all

# Tests

From your SpliceHoudini directory run:
* cd test; hython loadScenes.py ; cd -

Once tests are running well, you can start playing in Houdini !

# Licence

The license used for this DCC integration can be found in the root folder of this repository.

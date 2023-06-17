
## Simple Equalizer

This is a simple equalizer plugin built with JUCE framework.

### First Setup

- Clone the [JUCE](https://github.com/juce-framework/JUCE) repository into the folder you will be working on.
- Navigate to JUCE\extras\Projucer\Builds\ and choose between the IDE solutions folder depending on your system (MacOSX,LinuxMakeFile,VisualStudio).
- Open the solution file of the chosen build, then build and run it, the projucer app should open.
- Go to File>Global Paths and add the paths to the JUCE folder and modules (not necessary to add the User Modules path).
- Test that the paths work by pressing the "Re-scan Juce Modules" button.
- Go back to the main GUI and in new project select Basic from the plug-in section.
- Name the project and click "Create Project". That will generate the base project in the same folder as the JUCE folder.
- Inside your project folder add a .gitignore with the JuceLibraryCode and Builds folder names (also include .DS_Store if you are using mac).
- Initialize your git repository.

You are now all set to start building plugins with the JUCE framework!

### Framework Structure

There are 4 main files that you will be working on (inside Source): 

- PluginEditor.cpp      //layout objects definition (layout as in front-end items, like buttons, knobs, etc)
- PluginEditor.h        //layout objects declaration
- PluginProcessor.cpp   //Processing objects definition (processing as in back-end items, like freq range, etc)
- PluginProcessor.h     //Processing objects declaration



#Utilities to make comfortable the use of XCode with Tweaks

I recently abandoned [Coda 2](https://panic.com/coda/) as IDE for my Tweak [(I made a simple plug-In for that and ObjC syntax coloring-compention)](https://github.com/MP0w/TheosCodaPlugin) mainly because I wanted better ObjC completion and management .

Now I use Xcode where I made a project and I include my .xm(i) files (not added to any target) so I can use the simulator, Unit Testing , etc for my classes.

I will put here some utilities that help me using Xcode as a perfect IDE for Theos.

1. .xm and .xmi files template for Xcode are in the "Theos Files Template" folder and must be moved to ~/Library/Developer/Xcode/Templates/File\ Templates/ 
2. mpowMake is a simple script that you can use with the target (originally made for OSX) "external build system" , why? Xcode pass $(ACTION) to the script, where $(ACTION) is clean in case you are cleaning the project and anything if you build, to not edit the arguments manually to pass to make manually thhe script check if $1 exist if not put my arguments for the build (package install)
![](./externalBuildSystem)
3. .... 

# CSharp-MSTest-GNUMake

>This code is presented as an example only, since your tests and testing environments may require specialized scripting. This information should be taken only as an
>illustration of how one would set up tests with Sauce Labs, and any modifications will not be supported. For questions regarding Sauce Labs integration, please see 
>our documentation at [https://wiki.saucelabs.com/](https://wiki.saucelabs.com/).


Demonstrates how to use NUnit to run parallel tests on Sauce Labs platfrom using nmake as the build system. 

Uses [NuGet](http://docs.nuget.org/) as package manager.

#Dependencies:

* MS Visual Studio 2013 or later.
* [NuGet](https://dist.nuget.org/index.html) Plugin for Visual Studio
* [NuGet](https://dist.nuget.org/index.html) CLI executable installed in your path.
* [GNU-Make]http://gnuwin32.sourceforge.net/packages/make.htm
* You may need to add additional resources to the project (Selenium, etc.)

### Note: Use a Developer Command Prompt in order to access MSTest and MSBuild

#Setup:

* Install NuGet packages for the project: <br>
```cd Packages```<br>
```nuget.exe install ..\ParallelSelenium\packages.config```<br>

* Clean and rebuild project:<br>
```make prepare```

* Install GNU-Make

#Set Credentials:<br>
```set SAUCE_USERNAME=<sauce-username>```<br>
```set SAUCE_ACCESS_KEY=<sauce-access-key>```

#Run Tests in parallel on [Sauce](https://saucelabs.com/beta/dashboard/tests):<br>
```make all``` <br>






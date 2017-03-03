# Installation
We need to install two parts which are Visual Studio 2015 with Update 3 and Tooling preview to use .Net Core (for Windows).

Download Visual Studio 2015 with Update 3 
- [Install Japanese version](https://www.microsoft.com/net/core#windowsvs2015)
- [Install English version](https://www.visualstudio.com/downloads/?wt.mc_id=o~msft~mscom~jpvs2015)


Tooling preview that gives us the .NET Core command line tooling that we need.
You need to excute following command, if you get error and it says "Please repair Visual Studio 2015 Update 3,  
then install this product again"
```
SKIP_VSU_CHECK=1
```

and run 
```
dotnet
```

Now, you should be able to see below
```
C:\demos\CharacterCounter\test>dotnet

Microsoft .NET Core Shared Framework Host

  Version  : 1.0.1
  Build    : cee57bf6c981237d80aa1631cfe83cb9ba329f12

Usage: dotnet [common-options] [[options] path-to-application]

Common Options:
  --help                           Display .NET Core Shared Framework Host help.

  --version                        Display .NET Core Shared Framework Host versi
on.

Options:
  --fx-version <version>           Version of the installed Shared Framework to
use to run the application.
  --additionalprobingpath <path>   Path containing probing policy and assemblies
 to probe for.

Path to Application:
  The path to a .NET Core managed application, dll or exe file to execute.

If you are debugging the Shared Framework Host, set 'COREHOST_TRACE' to '1' in y
our environment.

To get started on developing applications for .NET Core, install .NET SDK from:
  http://go.microsoft.com/fwlink/?LinkID=798306&clcid=0x409
```

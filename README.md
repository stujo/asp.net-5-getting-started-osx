# ASP.NET 5 Getting Started on OSX

* Download the Release Candidate at [https://get.asp.net/](https://get.asp.net/). This will install the following for developing .NET applications:
  * .NET Execution Environment (DNX) - The .NET Execution Environments that you can use to build .NET applications on OS X.
  * .NET Version Manager (DNVM) - This utility is used to manage multiple versions of the .NET execution environment (DNX) on your machine. It is not recommended to install a DNX without the DNVM. DNVM is implemented as an sh file that is designed to be sourced into your shell.
 
* Under installation type I chose not to 'Add to bash' - Thinking that I'ld do that manually using a terminal tab preference by adding ``source dnvm`` to the tab setup, but that didn't work...

# Abort Abort :)
I really can't find the files that this pkg installed :(

* Trying manual install from [https://docs.asp.net/en/latest/getting-started/installing-on-mac.html](https://docs.asp.net/en/latest/getting-started/installing-on-mac.html)
* This silently DOES edit your ~/.bash_profile and insert itself. I took that out and then configured a terminal tab with that setup so as not to have this installed globally: The shell setup should have been ``source ~/.dnx/dnvm/dnvm.sh``

Tada!
```
[stu:~]$ dnvm
    ___  _  ___   ____  ___
   / _ \/ |/ / | / /  |/  /
  / // /    /| |/ / /|_/ / 
 /____/_/|_/ |___/_/  /_/  

.NET Version Manager - Version 1.0.0-rc2-15546
By Microsoft Open Technologies, Inc.

DNVM can be used to download versions of the .NET Execution Environment and manage which version you are using.
You can control the URL of the stable and unstable channel by setting the DNX_FEED and DNX_UNSTABLE_FEED variables.

Current feed settings:
Default Stable: https://www.nuget.org/api/v2
Default Unstable: https://www.myget.org/F/aspnetvnext/api/v2
Current Stable Override: <none>
Current Unstable Override: <none>

Use dnvm [help|-h|-help|--help]  to display help text.

```



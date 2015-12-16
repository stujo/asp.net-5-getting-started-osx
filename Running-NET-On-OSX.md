# BETA: How to Run a .NET Web Application on OSX

## Installing ASP.NET 5 On Mac OS X
* Mostly from here [https://docs.asp.net/en/latest/getting-started/installing-on-mac.html](https://docs.asp.net/en/latest/getting-started/installing-on-mac.html)

* Install Mono [http://www.mono-project.com/download/](http://www.mono-project.com/download/)
* Install DNVM Command Line
```
$ curl -sSL https://raw.githubusercontent.com/aspnet/Home/dev/dnvminstall.sh | DNX_BRANCH=dev sh && source ~/.dnx/dnvm/dnvm.sh
$ dnvm upgrade -r coreclr
$ dnvm upgrade -r mono
```
* Go to your app the folder with ``project.json`` (or if you don't have one use the [Yo Generator](../using-yo-generator.md)
```
$ dnu restore
$ dnx web
```
This should start the web application

* Visit the site [http://localhost:5000](http://localhost:5000)

Please let me know if this works 




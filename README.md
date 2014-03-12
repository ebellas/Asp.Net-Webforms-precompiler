#Precompiler for deployed Asp.Net Webforms (.Net 4.0)

Precompiles all aspx, ascx, ashx and other runtime compiled files.  Handy if you want to ship a web application but not include the raw files.

##Usage
1. Modify the `PhysicalPath` and `TargetPath` attributes of the Target element in the Precompiled.csproj file
2. You can define multile sites to precompile. Just duplicate the Target element and configure it appropriately.
3. Run msbuild, telling it which target to precompile, e.g
    ```
    C:\Windows\Microsoft.NET\Framework\v4.0.30319\msbuild Precompile.csproj  /t:Website1
    ``` 
 

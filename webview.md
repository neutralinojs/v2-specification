## Default browser component on Windows

v1.x implementation

These versions use MSHTML web browser component. In modern Windows versions, it will be IE11. 

v2.x implementation

v2 will use EdgeChromium as the web browser component. But, from the user's end we expect them to run the following command to get Neutralinojs apps working.

```cmd
CheckNetIsolation.exe LoopbackExempt -a -n="Microsoft.Win32WebViewHost_cw5n1h2txyewy"
```

The above command gives relavant permission for Neutralinojs (and all UWP applications) to access localhost from EdgeChromium.

# NP Plugin

## a simple win32 np-plugin sample

一个最简单的 np 插件示例，同时支持 windowed 和 windowless 两种模式，默认是 windowed 模式，可通过 windowless=1 属性指定为 windowless 模式。

## register the plugin for Firefox52 on Windows

``` bash
REG ADD HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\MozillaPlugins\npplugin.helloworld
REG ADD HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\MozillaPlugins\npplugin.helloworld /v Path /t REG_SZ /d %cd%\Debug\npsimple.dll
REG ADD HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\MozillaPlugins\npplugin.helloworld\MimeTypes
REG ADD HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\MozillaPlugins\npplugin.helloworld\MimeTypes\application/x-helloworld
```

## test page

np-hello.html

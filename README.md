> Catcher is a simple application focused on video games that allows you to reproduce/distribute your HTML/WEB games for Windows with greater ease, 
>compatibility and control over the system and the aesthetics of the experience that the developer is looking for. Catcher works with Webview2

## First release (1.2v)
---
### Features:

Management and modification of basic window appearance:
(Size, position, title)

-Full screen support

-WebGL support

-Initial state configuration with a "config.ini" file:
(Force full screen, initial window size, initial window position, initial window title)

-Loading custom icons for the taskbar and window with a "custom.ico" file
---

 >Catcher uses a minimum of 70 MB of memory when running.

 ##### catcher_1.2build_32_bits


 ---
 Some catcher functions have been fixed and made easier with simple messages. You can find them and their functions below or check the default index.html that comes with catcher in the "_game" folder.     
 ---
 ```
window.chrome.webview.postMessage
```
 // Windows state
 ```
{ action: "getWindowPosition" }
{ action: "getWindowSize" }
{ action: "setWindowPosition", x, y }
{ action: "setWindowSize", width, height }
{ action: "toggleFullscreen" }
{ action: "setWindowTitle", value: v }
{ action: "closeWindow" }
```

// Files
```
{ action: "readFile", path }
{ action: "writeFile", path, content: txt }
{ action: "LastFileWriteContent" }
{ action: "openFile", path }
```

// Windows
```
{ action: "newWindow" }
{ action: "newWindow", path }  //"_game/index2.html" 
```

// Browser Call
```
{ action: "callBrowser", url }
```

// Others
```
{ action: "get_document_in_pc_direction" }
```
---
## Construct 2

To export to Catcher with Construct 2, simply export your project to HTML5 and copy all generated content into the main folder containing "index.html."

>Catcher plugin 1.2v for construct 2

[Download C2Plugin](https://www.mediafire.com/file/pshni7hls65dhab/Catcher1_2v-Plugin_for_C2.zip/file)

[PeojectTemplateCapxC2](https://github.com/OLDGAME-Proyect/Catcher/tree/main/c2plugin/ExampleCAPX)



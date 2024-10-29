# cherry-snippet v2

## Intro

`cherry-snippet` It's with the help of [cherryTree](https://www.giuspen.com/cherrytree/) Note-taking software, a free and open-source **text fragment management tool** made by you

>[!Note]
>It is currently in beta and stable[cherry-snippet v1](https://github.com/sxzxs/cherry-snippet)
>
>_v1->v2 Improved: Preview with WebView2, D2D draw hook interface, add icon to List list_

- Code snippet **logging** and **quick searches** and **previews**
- The code snippet **is entered into the target window on the upper screen**  
    ![Show](https://raw.githubusercontent.com/pa-0/ahk.cherrysnippetv2/master/picture/sample.gif)
- Quick **Add Edits**
    ![Edit](https://raw.githubusercontent.com/pa-0/ahk.cherrysnippetv2/master/picture/edit.gif)
- Code snippet execution, currently executing python, ahk, bat, etc., for example, open Baidu
    ![Open Baidu](https://raw.githubusercontent.com/pa-0/ahk.cherrysnippetv2/master/picture/open_baidu.gif)
- Search supports **pinyin pinyin, simple pinning, small crane double, 86 five strokes, etc**
- hook. The mode is similar to the input method, and the cursor position is detected in real time  
    ![hook](https://raw.githubusercontent.com/pa-0/ahk.cherrysnippetv2/master/picture/HOOK.gif)

### Dependent environment

|Environment | version |
| --- | --- |
|system | To enable HTML preview**, you need win10** or installation **[webview2 runtime](https://msedge.sf.dl.delivery.mp.microsoft.com/filestreamingservice/files/3c9f7ac6-fb0a-4eb7-b1fd-44c57613a3f5/MicrosoftEdgeWebView2RuntimeInstallerX64.exe)** |
| ahk version | [AutoHotkey v2H](https://github.com/thqby/AutoHotkey_H/releases) |
| cherryTree.exe | [cherrytree Customized Baidu network disk](https://pan.baidu.com/s/1uDmzAsB_tgwexUccUjM0uA?pwd=bet2) Extract the code:bet2  <br/> [cherryTree Customized Blue Playing Cloud](https://wwob.lanzoum.com/iWmdr0mpjnfa) password:1bkm |
| dx  | [dx11 Download-dependent](https://zhangyue667.lanzouh.com/DirectXRepairEnhanced) |

### Installation Steps

1. Download zip，or git clone the repo
2. After that, execute cherry-snippet.ah2orcherrysnippet.exe
3. The first execution prompts for selection cherryTree.exe and data.ctb of the directory (cherrytree_0.99.51.0_win64_portable\mingw64\bin\cherrytree.exe)

### Directions for use

[A list of keys](https://htmlpreview.github.io/?https://github.com/pa-0/ahk.cherrysnippetv2/blob/master/README.html#general)

#### Normal search mode

- Open the search interface, default shift+enter
- To execute the code snippet, enter by default
- The current code snippet is entered into the target window, and the default is Ctrl+Enter
- Edit the current snippet with cherrytree, ctrl+e by default
- Copy the current code snippet to the system clipboard, default ctrl+c

#### hookSearch mode

- Open the hook interface, default shift+space
- The current code snippet is entered into the target window, default enter

### Plug-ins

#### /cal calculator

`For example: /cal 100+100`

#### /cd Dictionary translation

`For example: /cd I can translate in real time`  
Press Enter, enter into the target window  
Ctrl+Enter, and convert the English of the pair to the variable name

#### Customize the listview icon

1. Modify the attributes of the node in cherrytree and add the keyword "icon:Baidu" to the tag
2. After setting the name using the above method, you need to place the files in the format of lnk, png, icon, etc. with the corresponding name to the /icons/tree directory

![img](https://img2023.cnblogs.com/blog/2850002/202302/2850002-20230222001733261-592590197.png)

![img](https://img2023.cnblogs.com/blog/2850002/202302/2850002-20230222001212880-2097820494.png)

If the parent node has an icon, the child node also inherits  
**icon: xx must be written to the end**

#### Mask nodes and sub nodes

Modify the properties of the node in cherrytree and add the "mask" keyword to the tag, as shown in the figure above

#### Precautions

- Generally, the .ctb file and export path should not be set to the C drive (unknown permission issue)
- The cherrytree setting can speed up the jump`Enable the system tray`  
    ![cherrytree Enable the system tray](https://raw.githubusercontent.com/pa-0/ahk.cherrysnippetv2/master/picture/cherrytree%E8%AE%BE%E7%BD%AE.png)

### TODO

- The shortcut key setting UI is complete
- HTML format content is stored on the clipboard

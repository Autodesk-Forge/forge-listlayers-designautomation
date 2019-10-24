# ListLayers CRX Plug-in for Design Automation

[![Design Automation](https://img.shields.io/badge/Design%20Automation-v3-green.svg)](http://developer.autodesk.com/)
[![visual studio](https://img.shields.io/badge/Visual%20Studio-2017-yellowgreen.svg)](https://www.visualstudio.com/)
[![AutoCAD](https://img.shields.io/badge/AutoCAD-2020-DF1B22.svg)](http://developer.autodesk.com/)
[![License](https://img.shields.io/:license-mit-red.svg)](http://opensource.org/licenses/MIT)


## Description

An AutoCAD CRX Plug-in that implements an AutoCAD custom command named TEST. This command extracts the layer names from the current drawing and saves them to a text file.

## Dependencies

-  [Visual Studio](https://visualstudio.microsoft.com/downloads/). This sample was created in Visual Studio 2017.
-  [AutoCAD .NET API](https://www.nuget.org/packages/AutoCAD.NET/23.1.0). This sample was built using the AutoCAD 2020 .NET API.

## Build the project

1. Open *command.sln* in Visual Studio.

2. In Visual Studio, in the Solution Explorer, right-click the project name. A menu displays.

3. Click **Manage NuGet Packages**. The Manage Packages for Solution dialog displays.

4. Click **Restore**, which is on the top-right of the dialog. The packages are downloaded and restored.

5. Build the solution. 

## Testing whether the custom command works

We recommend that you test the custom command on your local machine before you use it in Design Automation.

1. Start AutoCAD. (This code sample was tested with AutoACD 2020)

2. Open a drawing file. You can use any of the drawing files from [the AutoCAD samples page](https://knowledge.autodesk.com/support/autocad/downloads/caas/downloads/content/autocad-sample-files.html).

3. On the AutoCAD command line, enter NETLOAD.

4. Select *command.dll* that you built in the previous section.

5. On the command line, enter TEST. If the plug-in executes as designed, a text file containing the layer names is generated. The file is typically saved in the folder that you most recently interacted with in AutoCAD.

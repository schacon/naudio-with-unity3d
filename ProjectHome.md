When I want to record sound in unity3D with naudio library, it does not work, then I find the official naudio dll is built with csc.exe and .net framework 4.0, and unity3d only support mono and .net framework 2.0, so I begin to compile naudio with mono and .net framework 2.0, after changing a lot of syntax differences, it can be compiled with no error, then I test the sound playing and recording, and it works.

You can use the dll (based on naudio-d3f179cf7367) in the project, please remember to config in unity3D with
File - Build Settings - Player Settings - Settings for PC and Mac Standalone - Optimization - Api Compatibility Level
to .NET 2.0.
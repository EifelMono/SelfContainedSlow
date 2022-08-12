# SelfContainedSlow 

Defenders slows down .NET 6.0 SelfContained singleexe files

## Code and Build

The c# program contains nothing

```csharp
Console.WriteLine("Hello, World!");
Console.ReadLine();
```

```console
dotnet publish -c Release -r win-x64 --output ./artifacts --self-contained true -p:PublishSingleFile=true -p:IncludeAllContentForSelfExtract=true -p:IncludeAllContentForSelfExtract=true -p:CopyOutputSymbolsToPublishDirectory=false -p:EnableCompressionInSingleFile=true

```


## How to Test

* Clone the repository to your computer "git clone https://github.com/EifelMono/SelfContainedSlow.git" 
* Download [.NET 6.0 SDK](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/sdk-6.0.400-windows-x64-installer) and install
* Run build.cmd
* Execute artifacts\SelfContainedSlow.exe


## Result

Video when I open the file property dialog or starts the program

#### gif
![Alt Text](https://github.com/EifelMono/SelfContainedSlow/blob/main/images/2022-08-11_23-00-57.gif)

#### mp4
[Download video with better quality](https://github.com/EifelMono/SelfContainedSlow/blob/main/images/2022-08-11_23-00-25.mp4)


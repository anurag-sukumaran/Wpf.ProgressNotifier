# WPF.ProgressNotifier     

![progress_notifier_icon](Wpf.ProgressNotifier.Sample/Images/progress_notifier_icon.png)

This is a WPF control to show the progress of a long (aync) running task

[![Nuget](https://img.shields.io/nuget/v/Fluent.Ribbon.svg?style=flat-square)](https://www.nuget.org/packages/WPF.ProgressNotifier)

<div align="center">
 
![progress_notifier](Wpf.ProgressNotifier.Sample/Images/progress_notifier.gif)

</div>

## Installation

Available on [Nuget](https://www.nuget.org/packages/WPF.ProgressNotifier/) 

```bash
Install-Package WPF.ProgressNotifier 
```

## Usage
Add Namespace
```xaml
 <xmlns:notification="clr-namespace:RbCreation.Wpf.ProgressNotifier;assembly=RbCreation.Wpf.ProgressNotifier" 
  xmlns:System="clr-namespace:System;assembly=mscorlib"  />
```
Add Control 
```xaml
<notification:ProgressNotifier x:Name="progress"  IntervalNotifier="2"   Foreground="Black" FontSize="14" FontFamily="Arial"
                                       IsBusy="True" VerticalAlignment="Center" HorizontalAlignment="Stretch" SpinnerHeight="30" SpinnerWidth="30" >
            <notification:ProgressNotifier.ProgressTextSource>
                <System:String>Retrieving..</System:String>
                <System:String>Validating the credentials..</System:String>
                <System:String>Retrieving Data..</System:String>
                <System:String>Connecting to the server..</System:String>
                <System:String>Fetching..</System:String>
            </notification:ProgressNotifier.ProgressTextSource>
        </notification:ProgressNotifier>
```
Set Busy (The spinner will run according to this bindable property)
```xaml
 IsBusy="True 
```

## Sample

Clone the [sample](https://github.com/anurag-sukumaran/Wpf.ProgressNotifier.git) code


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
Copyright © RbCreation 2021


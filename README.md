# TestConnectedApp
this is how to get the new Connected App template up and running in Visual Studio for Mac Preview 1


How to run this solution in the iOS simulator, from scratch:
------------------------------------------------------------

1. Install .NET Core 1.1
  * follow ALL the steps [here] (https://www.microsoft.com/net/core#macos)
2. Install .NET Core 1.0 also (that's what the template uses)
  * [under LTS & SDK] (https://www.microsoft.com/net/download/core)
3. Pick the "Multiple" run configuration (instead of TestConnnectedApp.iOS for example) and Run!


What I did to make this solution:
------------------------------------------------------------

1. Create new solution from the Connected App template in VS for Mac
  * New Project > Multiplatform > App > Connected App
2. Create a new Solution Run Configuration 
  * VS for Mac now supports [Multi-Process Debugging] (https://developer.xamarin.com/releases/vs-mac/preview/vs-mac-preview1/#Multi-Process_Debugging) so you can run the Rest API backend project AND the iOS/Android client at the same time!
  * Solution > Options > Run > Configurations > New
  * Name it "Multiple" and check the boxes next to the mobile head project + MobileAppService project 
  

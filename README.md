# HelloXamarinUITest
A small sample app that uses Xamarin UITests framework

### To run the tests on AppCenter Test:

```
npm install -g appcenter-cli
appcenter login

//Android
appcenter test run uitest --app "a.winterdoug/HelloXamarinUITest.Android" --devices fa79afac --app-path "path\to\com.companyname.HelloXamarinUITest_Signed.apk" --test-series "master" --locale "en_US" --build-dir "path\to\HelloXamarinUITest\HelloXamarinUITest\HelloXamarinUITest.UITest\bin\UITests" --uitest-tools-dir "%userprofile%\.nuget\packages\xamarin.uitest\2.2.6\tools"

//iOS
appcenter test run uitest --app "a.winterdoug/HelloXamarinUITest.iOS" --devices cd5df228 --app-path "path\to\UITests\HelloXamarinUITest.iOS.ipa" --test-series "master" --locale "en_US" --build-dir "path\to\HelloXamarinUITest\HelloXamarinUITest\HelloXamarinUITest.UITest\bin\UITests" --uitest-tools-dir "%userprofile%\.nuget\packages\xamarin.uitest\2.2.6\tools"
```

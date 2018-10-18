# HelloXamarinUITest
A small sample app that uses Xamarin UITest framework

### To build and run the tests on AppCenter Test

- Select the "UITests" build configuration
- Build the solution
- iOS IPA file will be genrated on build (nothing to do)
- For Android, generate the signed APK (Archive)

```
npm install -g appcenter-cli
appcenter login

//Android
appcenter test run uitest --app "ACCOUNT/HelloXamarinUITest.Android" --devices DEVICEID --app-path "path\to\com.companyname.HelloXamarinUITest_Signed.apk" --test-series "master" --locale "en_US" --build-dir "path\to\HelloXamarinUITest\HelloXamarinUITest\HelloXamarinUITest.UITest\bin\UITests" --uitest-tools-dir "%userprofile%\.nuget\packages\xamarin.uitest\2.2.6\tools"

//iOS
appcenter test run uitest --app "ACCOUNT/HelloXamarinUITest.iOS" --devices DEVICEID --app-path "path\to\UITests\HelloXamarinUITest.iOS.ipa" --test-series "master" --locale "en_US" --build-dir "path\to\HelloXamarinUITest\HelloXamarinUITest\HelloXamarinUITest.UITest\bin\UITests" --uitest-tools-dir "%userprofile%\.nuget\packages\xamarin.uitest\2.2.6\tools"
```

### Packages used in this repository
- Xamarin.Forms 3.2.0.871581
- Xamarin.TestCloud.Agent 0.21.7
- Xamarin.UITest 2.2.6
- NUnit 2.6.4
- NUnitTestAdapter 2.1.1

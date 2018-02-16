This repository is experimental custom msbuild SDK resolver for Xamarin.Android.

These samples don't build yet.

- HelloWorld - specifies Xamarin.Android.Sdk indicating that there is an
  installed SDK under $mono_prefix/lib/mono/msbuild/15.0/bin/Sdk. 
  (To do this, run `ln -s $(PWD)/build $(mono_prefix)/lib/mono/msbuild/15.0/bin/Sdk/Xamarin.Android.Sdk`).
- CustomSdkNuGet - specifies name.atsushieno.xamarin.android.sdk indicating
  that it uses name.atsushieno.xamarin.android.sdk nuget package to resolve
  its SDK to build with. In the future we might become able to ship MSBuild
  build tasks individually, isolated from large Xamarin.Android distribution.
- SimulatePreviewApiFromNuGet - it is to resolve custom framework too,
  not just custom SDK. Maybe it should rather become another package.


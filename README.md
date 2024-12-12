# How-to-customize-the-Image-size-in-.NET-MAUI-TabView
This repository contains a sample explaining how to Customize the Image size in .NET MAUI TabView.

### ImageSize support in .NET MAUI TabView

The `ImageSize` property allows you to customize the size of images in the TabView control, enhancing its visual appeal and ensuring consistency.

The following code example illustrate how to Customize ImageSize in SfTabView.

### XAML

```
    <tabView:SfTabView>
    <tabView:SfTabItem ImageSize="50"/>
    </tabView:SfTabView> 
```

### C#

```
    var tabView = new SfTabView();
    var tabItems = new TabItemCollection
    {
    new SfTabItem()
    {
        ImageSize = 50,
    }
    };
    tabView.Items = tabItems; 
```
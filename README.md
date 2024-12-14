# How-to-customize-the-Image-size-in-.NET-MAUI-TabView
This repository contains a sample explaining how to Customize the Image size in .NET MAUI TabView.

### ImageSize support in .NET MAUI TabView

The `ImageSize` property allows you to customize the size of images in the TabView control, enhancing its visual appeal and ensuring consistency.

The following code example illustrate how to Customize ImageSize in SfTabView.

### XAML

```
     <Grid VerticalOptions="FillAndExpand">
     <tabView:SfTabView x:Name="tabview" TabBarHeight="100">
         <tabView:SfTabItem ImageSize="50" Header="Jackson" ImageSource="jackson.png">
             <StackLayout Padding="10">
                 <Label Text="Welcome, Jackson!" 
                    FontSize="18" 
                    HorizontalOptions="Center" />
                 <Label Text="Here is your profile information." 
                    FontSize="14" 
                    HorizontalOptions="Center" />
             </StackLayout>
         </tabView:SfTabItem>

         <tabView:SfTabItem ImageSize="50" Header="Liam" ImageSource="liam.png">
             <StackLayout Padding="10">
                 <Label Text="Welcome, Liam!" 
                    FontSize="18" 
                    HorizontalOptions="Center" />
                 <Label Text="Here is your profile information." 
                    FontSize="14" 
                    HorizontalOptions="Center" />
             </StackLayout>
        </tabView:SfTabItem>
     </tabView:SfTabView>
     </Grid>
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
# Selected item customization in ListView

The SfListView supports customizing the selection background color for the selected items by using the [SfListView.SelectedItemTemplate](https://help.syncfusion.com/cr/cref_files/xamarin/Syncfusion.SfListView.XForms~Syncfusion.ListView.XForms.SfListView~SelectedItemTemplate.html) if the background color is set to view loaded in the [SfListView.ItemTemplate](https://help.syncfusion.com/cr/cref_files/xamarin/Syncfusion.SfListView.XForms~Syncfusion.ListView.XForms.SfListView~ItemTemplate.html).

```
<ContentPage  xmlns:syncfusion="clr-namespace:Syncfusion.ListView.XForms;assembly=Syncfusion.SfListView.XForms">
  <syncfusion:SfListView x:Name="listView">
   <syncfusion:SfListView.SelectedItemTemplate>
    <DataTemplate>
     <Grid x:Name="grid" BackgroundColor="RoyalBlue">
      <Grid.RowDefinitions>
         <RowDefinition Height="*" />
         <RowDefinition Height="*" />
         <RowDefinition Height="1" />
       </Grid.RowDefinitions>
      <Label Text="{Binding SongTitle}" />
      <Label Text="{Binding SongAuther}" Grid.Row="1"/>
      <Frame Grid.Row="2" HasShadow="True" HeightRequest="1"/>
     </Grid>
    </DataTemplate>
   </syncfusion:SfListView.SelectedItemTemplate>
  </syncfusion:SfListView>
</ContentPage>
```
To know more about selection in ListView, please refer our documentation[here](https://help.syncfusion.com/xamarin/sflistview/selection).


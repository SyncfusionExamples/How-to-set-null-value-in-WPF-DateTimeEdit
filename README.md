# How to Set Null Value in WPF DateTimeEdit
This example demonstrates how to allow null values in the Syncfusion WPF DateTimeEdit control. By default, DateTimeEdit requires a valid date and time value, but in many real-world scenarios, you may want to allow users to clear the value or represent an empty state. This is especially useful in forms where the date field is optional or when you need to reset the control programmatically.

## Why This Is Useful
- **Optional Fields**: Ideal for forms where date selection is not mandatory.
- **Reset Functionality**: Allows clearing the date programmatically.
- **Better UX**: Displays custom text when no date is selected.

## Key Properties
- **IsEmptyDateEnabled**: Enables empty date selection.
- **NullValue**: Represents the null state.
- **NoneDateText**: Custom text displayed when no date is selected.
- **ShowMaskOnNullValue**: Controls whether the mask is shown when the value is null.

## Code Example
**XAML**
```XAML
<syncfusion:DateTimeEdit x:Name="dateTimeEdit"
                         Height="23"
                         Width="150"
                         IsEmptyDateEnabled="True"
                         IsVisibleRepeatButton="True"
                         NullValue="{x:Null}"
                         NoneDateText="No date is selected"
                         ShowMaskOnNullValue="False" />
```

**C#**
```C#
DateTimeEdit dateTime = new DateTimeEdit
{
    Height = 25,
    Width = 150,
    IsEmptyDateEnabled = true,
    IsVisibleRepeatButton = true,
    NullValue = null,
    NoneDateText = "No date is selected",
    ShowMaskOnNullValue = false
};

this.Content = dateTime;
```

## Output

![Null value in WPF DateTimeEdit](output.png)

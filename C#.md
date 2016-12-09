# C# 4.5

## Tips and Tricks

Get property value by the name of the property

```csharp
private object GetPropValue(object src, string propName)
{
    return src.GetType().GetProperty(propName, BindingFlags.Default).GetValue(src, null);
}
```

!Note If the property type is nullable then the GetProperty() method returns NULL 
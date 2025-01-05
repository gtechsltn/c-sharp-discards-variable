# CSharp Discards Variable

Discards - C# Fundamentals

https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/functional/discards

```
_ = DateTime.TryParse("02/29/2019", out result);  
```

C# Hidden Gems - Discards Variable (_)

https://www.c-sharpcorner.com/blogs/c-sharp-hidden-gems-sharp1-discards-variable

## Without Discards Variable
```
DateTime result;  
if (DateTime.TryParse("02/29/2019", out result))  
{  
    Console.WriteLine("Date is valid");  
}  
else  
{  
    Console.WriteLine("Date is not valid");  
}  
```

## With Discards Variable
```
if (DateTime.TryParse("02/29/2019", out _))  
{  
    Console.WriteLine("Date is valid");  
}  
else  
{  
    Console.WriteLine("Date is not valid");  
}
```

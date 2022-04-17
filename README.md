## xxHash Implementation in C#

Adds extension methods for xxHash
- GetXxHash32
- GetXxHash64

to the following types:
- byte[]
- Span<byte>
- ReadOnlySpan<byte>

  
**Can be used as follows:**
```csharp
using xxHash;
  
byte[] data = Encoding.UTF8.GetBytes("Hello xxHash");
ulong hash = data.GetXxHash64();
```
  
  
***seed*** is an optional parameter
```csharp
using xxHash;
  
byte[] data = Encoding.UTF8.GetBytes("Hello xxHash");
ulong hash = data.GetXxHash64(12345);
```


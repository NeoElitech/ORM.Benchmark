```

BenchmarkDotNet v0.13.8, Windows 11 (10.0.22000.2295/21H2/SunValley)
12th Gen Intel Core i7-12800H, 1 CPU, 20 logical and 14 physical cores
.NET SDK 7.0.306
  [Host]     : .NET 6.0.21 (6.0.2123.36311), X64 RyuJIT AVX2
  DefaultJob : .NET 6.0.21 (6.0.2123.36311), X64 RyuJIT AVX2


```
| Method                              | Mean     | Error     | StdDev    | Rank | Gen0   | Allocated |
|------------------------------------ |---------:|----------:|----------:|-----:|-------:|----------:|
| Dapper_UpdateSpecifcPropertiesAsync | 1.570 ms | 0.0179 ms | 0.0167 ms |    1 |      - |  17.17 KB |
| EFCore_UpdateSpecifcPropertiesAsync | 1.767 ms | 0.0091 ms | 0.0081 ms |    2 | 5.8594 |  73.97 KB |

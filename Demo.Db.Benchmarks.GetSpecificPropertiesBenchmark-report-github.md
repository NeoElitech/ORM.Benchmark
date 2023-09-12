```

BenchmarkDotNet v0.13.8, Windows 11 (10.0.22000.2295/21H2/SunValley)
12th Gen Intel Core i7-12800H, 1 CPU, 20 logical and 14 physical cores
.NET SDK 7.0.306
  [Host]     : .NET 6.0.21 (6.0.2123.36311), X64 RyuJIT AVX2
  DefaultJob : .NET 6.0.21 (6.0.2123.36311), X64 RyuJIT AVX2


```
| Method                                      | Mean     | Error    | StdDev   | Rank | Gen0   | Gen1   | Allocated |
|-------------------------------------------- |---------:|---------:|---------:|-----:|-------:|-------:|----------:|
| Dapper_SelectSpecifcPropertiesAsync         | 15.51 μs | 0.208 μs | 0.194 μs |    1 | 0.7629 |      - |   9.48 KB |
| DapperFastCrud_SelectSpecifcPropertiesAsync | 19.85 μs | 0.348 μs | 0.372 μs |    2 | 1.2512 | 0.0305 |  15.38 KB |
| EFCore_SelectSpecifcPropertiesAsync         | 94.47 μs | 1.864 μs | 4.092 μs |    3 | 5.0049 | 0.8545 |  61.43 KB |

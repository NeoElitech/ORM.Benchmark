```

BenchmarkDotNet v0.13.8, Windows 11 (10.0.22000.2295/21H2/SunValley)
12th Gen Intel Core i7-12800H, 1 CPU, 20 logical and 14 physical cores
.NET SDK 7.0.306
  [Host]     : .NET 6.0.21 (6.0.2123.36311), X64 RyuJIT AVX2
  DefaultJob : .NET 6.0.21 (6.0.2123.36311), X64 RyuJIT AVX2


```
| Method                     | Mean     | Error     | StdDev    | Rank | Gen0   | Allocated |
|--------------------------- |---------:|----------:|----------:|-----:|-------:|----------:|
| Dapper_InsertAsync         | 1.563 ms | 0.0164 ms | 0.0146 ms |    1 |      - |  14.46 KB |
| DapperFastCrud_InsertAsync | 1.578 ms | 0.0269 ms | 0.0224 ms |    1 |      - |  22.08 KB |
| EFCore_InsertAsync         | 1.684 ms | 0.0264 ms | 0.0234 ms |    2 | 3.9063 |  68.34 KB |

```

BenchmarkDotNet v0.13.8, Windows 11 (10.0.22000.2295/21H2/SunValley)
12th Gen Intel Core i7-12800H, 1 CPU, 20 logical and 14 physical cores
.NET SDK 7.0.306
  [Host]     : .NET 6.0.21 (6.0.2123.36311), X64 RyuJIT AVX2
  DefaultJob : .NET 6.0.21 (6.0.2123.36311), X64 RyuJIT AVX2


```
| Method                     | Mean     | Error     | StdDev    | Rank | Gen0   | Allocated |
|--------------------------- |---------:|----------:|----------:|-----:|-------:|----------:|
| Dapper_UpdateAsync         | 1.574 ms | 0.0191 ms | 0.0169 ms |    1 |      - |  21.37 KB |
| DapperFastCrud_UpdateAsync | 1.575 ms | 0.0099 ms | 0.0088 ms |    1 |      - |  22.64 KB |
| EFCore_UpdateAsync         | 1.716 ms | 0.0128 ms | 0.0120 ms |    2 | 3.9063 |  68.84 KB |

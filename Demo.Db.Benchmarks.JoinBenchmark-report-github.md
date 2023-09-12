```

BenchmarkDotNet v0.13.8, Windows 11 (10.0.22000.2295/21H2/SunValley)
12th Gen Intel Core i7-12800H, 1 CPU, 20 logical and 14 physical cores
.NET SDK 7.0.306
  [Host]     : .NET 6.0.21 (6.0.2123.36311), X64 RyuJIT AVX2
  DefaultJob : .NET 6.0.21 (6.0.2123.36311), X64 RyuJIT AVX2


```
| Method              | Mean      | Error    | StdDev   | Rank | Gen0   | Gen1   | Allocated |
|-------------------- |----------:|---------:|---------:|-----:|-------:|-------:|----------:|
| DapperFastCrud_Join |  54.98 μs | 1.099 μs | 2.758 μs |    1 | 3.1738 | 0.1221 |  40.17 KB |
| EFCore_Join         | 158.97 μs | 2.965 μs | 5.193 μs |    2 | 5.6152 | 0.7324 |  68.85 KB |

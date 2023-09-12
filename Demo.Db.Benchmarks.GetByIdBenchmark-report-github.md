```

BenchmarkDotNet v0.13.8, Windows 11 (10.0.22000.2295/21H2/SunValley)
12th Gen Intel Core i7-12800H, 1 CPU, 20 logical and 14 physical cores
.NET SDK 7.0.306
  [Host]     : .NET 6.0.21 (6.0.2123.36311), X64 RyuJIT AVX2
  DefaultJob : .NET 6.0.21 (6.0.2123.36311), X64 RyuJIT AVX2


```
| Method                           | Mean     | Error    | StdDev   | Rank | Gen0   | Gen1   | Allocated |
|--------------------------------- |---------:|---------:|---------:|-----:|-------:|-------:|----------:|
| Dapper_QuerySingleOrDefaultAsync | 16.24 μs | 0.177 μs | 0.147 μs |    1 | 0.7935 |      - |   9.83 KB |
| DapperFastCrud_GetAsync          | 22.53 μs | 0.403 μs | 0.377 μs |    2 | 1.4038 | 0.0305 |  17.57 KB |
| EFCore_FirstOrDefaultAsync       | 86.96 μs | 1.709 μs | 2.281 μs |    3 | 4.7607 | 0.8545 |  58.84 KB |
| EFCore_SingleOrDefaultAsync      | 88.99 μs | 1.758 μs | 1.805 μs |    4 | 4.7607 | 0.8545 |  58.84 KB |

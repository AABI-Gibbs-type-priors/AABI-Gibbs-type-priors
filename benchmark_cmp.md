# Benchmark Report for *GibbsTypePriors*

## Job Properties
* Time of benchmarks:
    - Target: 30 Apr 2020 - 17:48
    - Baseline: 30 Apr 2020 - 17:49
* Package commits:
    - Target: 689bd0
    - Baseline: 069a63
* Julia commits:
    - Target: 381693
    - Baseline: 381693
* Julia command flags:
    - Target: None
    - Baseline: None
* Environment variables:
    - Target: None
    - Baseline: None

## Results
A ratio greater than `1.0` denotes a possible regression (marked with :x:), while a ratio less
than `1.0` denotes a possible improvement (marked with :white_check_mark:). Only significant results - results
that indicate possible regressions or improvements - are shown below (thus, an empty table means that all
benchmark results remained invariant between builds).

| ID                              | time ratio                   | memory ratio  |
|---------------------------------|------------------------------|---------------|
| `["Cnk", "recursive_arb"]`      | 0.88 (5%) :white_check_mark: | 1.05 (1%) :x: |
| `["Cnk", "recursive_arb_long"]` |                   0.98 (5%)  | 1.07 (1%) :x: |

## Benchmark Group List
Here's a list of all the benchmark groups executed by this job:

- `["Cnk"]`
- `["Vnk"]`
- `["utf8"]`

## Julia versioninfo

### Target
```
Julia Version 1.4.1
Commit 381693d3df* (2020-04-14 17:20 UTC)
Platform Info:
  OS: Linux (x86_64-pc-linux-gnu)
      Ubuntu 18.04.4 LTS
  uname: Linux 5.3.0-46-generic #38~18.04.1-Ubuntu SMP Tue Mar 31 04:17:56 UTC 2020 x86_64 x86_64
  CPU: Intel(R) Core(TM) i7-8665U CPU @ 1.90GHz: 
              speed         user         nice          sys         idle          irq
       #1  4200 MHz    3634009 s       2431 s    1003244 s   28861560 s          0 s
       #2  4200 MHz    3842530 s       3288 s    1006373 s   28580401 s          0 s
       #3  4200 MHz    3984236 s       1492 s    1013235 s   28560971 s          0 s
       #4  4200 MHz    4029143 s       1927 s    1011533 s   28439327 s          0 s
       #5  4200 MHz    4008652 s       2531 s    1002150 s   28455856 s          0 s
       #6  4200 MHz    3909294 s       2678 s     988382 s   28675981 s          0 s
       #7  4200 MHz    3874568 s        994 s    1014147 s   28578069 s          0 s
       #8  4200 MHz    3799549 s       1724 s    1017153 s   28710435 s          0 s
       
  Memory: 31.242061614990234 GB (9695.32421875 MB free)
  Uptime: 891641.0 sec
  Load Avg:  1.2890625  1.19921875  1.16015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-8.0.1 (ORCJIT, skylake)
```

### Baseline
```
Julia Version 1.4.1
Commit 381693d3df* (2020-04-14 17:20 UTC)
Platform Info:
  OS: Linux (x86_64-pc-linux-gnu)
      Ubuntu 18.04.4 LTS
  uname: Linux 5.3.0-46-generic #38~18.04.1-Ubuntu SMP Tue Mar 31 04:17:56 UTC 2020 x86_64 x86_64
  CPU: Intel(R) Core(TM) i7-8665U CPU @ 1.90GHz: 
              speed         user         nice          sys         idle          irq
       #1  3035 MHz    3637444 s       2431 s    1003531 s   28862049 s          0 s
       #2  2928 MHz    3842660 s       3288 s    1006421 s   28584434 s          0 s
       #3  2995 MHz    3984419 s       1492 s    1013311 s   28564919 s          0 s
       #4  3014 MHz    4029239 s       1927 s    1011599 s   28443361 s          0 s
       #5  3117 MHz    4008886 s       2531 s    1002192 s   28459784 s          0 s
       #6  3001 MHz    3909417 s       2678 s     988435 s   28680017 s          0 s
       #7  3090 MHz    3874680 s        994 s    1014190 s   28582107 s          0 s
       #8  2977 MHz    3799908 s       1724 s    1017196 s   28714232 s          0 s
       
  Memory: 31.242061614990234 GB (9697.41015625 MB free)
  Uptime: 891683.0 sec
  Load Avg:  1.4921875  1.251953125  1.1796875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-8.0.1 (ORCJIT, skylake)
```
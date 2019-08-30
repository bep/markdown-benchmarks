# Markdown Benchmarks

Benchmarks adapted from https://github.com/yuin/goldmark/

Run on my 2,7 GHz Intel Core i5 8GB MacBook:

```bash
▶ go test -run="NONE" -bench="Benchmark" -test.benchmem=true
goos: darwin
goarch: amd64
pkg: github.com/bep/markdown-benchmarks
BenchmarkMarkdown/Blackfriday-v1-4         	     300	   4044523 ns/op	 1435767 B/op	    5362 allocs/op
BenchmarkMarkdown/Blackfriday-v2-4         	     300	   5296334 ns/op	 3341237 B/op	   20057 allocs/op
BenchmarkMarkdown/GoldMark-4               	     300	   5892282 ns/op	 2608502 B/op	   13863 allocs/op
BenchmarkMarkdown/CommonMark-4             	     200	   6999306 ns/op	 2769000 B/op	   18832 allocs/op
BenchmarkMarkdown/GoMarkdown-4             	      10	 133824801 ns/op	 2199848 B/op	   22175 allocs/op
PASS
ok  	github.com/bep/markdown-benchmarks	9.810s
```


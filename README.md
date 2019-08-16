# Markdown Benchmarks

Benchmarks adapted from https://github.com/yuin/goldmark/

Run on my 2,7 GHz Intel Core i5 8GB MacBook:

```bash
▶ go test -run="NONE" -bench="Benchmark"  -test.benchmem=true .
goos: darwin
goarch: amd64
pkg: github.com/bep/markdown-benchmarks
BenchmarkMarkdown/Blackfriday-v1-4         	     300	   4114349 ns/op	 1435509 B/op	    5361 allocs/op
BenchmarkMarkdown/Blackfriday-v2-4         	     300	   5314095 ns/op	 3338895 B/op	   20057 allocs/op
BenchmarkMarkdown/GoldMark-4               	     200	   6374712 ns/op	 2608445 B/op	   13863 allocs/op
BenchmarkMarkdown/CommonMark-4             	     200	   6966669 ns/op	 2770433 B/op	   18831 allocs/op
BenchmarkMarkdown/GoMarkdown-4             	      10	 133411429 ns/op	 2199855 B/op	   22175 allocs/op
PASS
ok  	github.com/bep/markdown-benchmarks	9.394s
```


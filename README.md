# sqltee

[![Build Status](https://cloud.drone.io/api/badges/sqltee/sqltee/status.svg)](https://cloud.drone.io/sqltee/sqltee)
[![Go Reference](https://pkg.go.dev/badge/github.com/sqltee/sqltee.svg)](https://pkg.go.dev/github.com/sqltee/sqltee)

SQL [database/sql/driver][] wrapping, queries interpolation, execution time
and arguments logging (values, named values, transaction options) for Go.

Source files are distributed under the BSD-style license.

[database/sql/driver]: https://golang.org/pkg/database/sql/driver

## About

The software is considered to be at a alpha level of readiness,
its extremely slow and allocates a lots of memory.

## Benchmark

```sh
$ go test -run ^NOTHING -bench BenchmarkGob\$
goos: linux
goarch: amd64
pkg: github.com/sqltee/sqltee/examples/teegob
cpu: 11th Gen Intel(R) Core(TM) i7-1165G7 @ 2.80GHz
BenchmarkGob/gob_test.go:53/query_from_existing_table-8                 2379        510046 ns/op
PASS
ok      github.com/sqltee/sqltee/examples/teegob 1.270s
```

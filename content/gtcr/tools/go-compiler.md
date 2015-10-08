+++
weight = 101
Categories = ["Golang"]
Description = ""
Tags = ["golang"]
date = "2015-09-21T16:58:01+08:00"
menu = "ghg-main"
title = "第一章：Go编译器"
parttitle = "Golang的那些事儿 - 第二部分：工具"
prev = "intro"
next = "overview"
booktitle = "Golang - The Complete Reference"
displaynav = "true"

+++

```
package main

import (
	"fmt"
	"runtime"
)

type Point struct {
	x int
	y int
}

// main函数
func main() {
	var sl = []Point{{3, 4}, {5, 6}}
	var m = map[Point]string{
		{3,4}:"foo1",
		{5,6}:"foo2",
	}
	fmt.Println(sl)
	fmt.Println(m)
	fmt.Println(runtime.GOMAXPROCS(-1))
	fmt.Println(runtime.NumGoroutine())
}
```

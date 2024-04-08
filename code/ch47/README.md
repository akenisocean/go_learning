## 性能测试 bechmark+pporf

步骤：
1. 生成一个cpu的性能测试文件,名称伟cpu.prof
```shell
go test -bench=. -cpuprofile=cpu.prof
```
2. pprof命令分析
```shell
go tool pprof cpu.prof
```
常用pprof命令
- cpu性能测试： go test -bench=. -cpuprofile=cpu.prof
- 内存性能测试： go test -bench=. -memprofile=mem.prof
- 工具： go tool  pprof cpu.prof
- 工具： go tool pprof mem.prof
- 

http://docscn.studygolang.com/pkg/net/http/pprof/


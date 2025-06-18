# ⚡ Optimisation en Julia

## Benchmark

```julia title="benchmark.jl"
using BenchmarkTools
```

@btime sum($(rand(1000)))  # ~1.5 μs (vs Python ~150 μs)

## Parallelisation

```julia
using Distributed
addprocs(4)

@distributed for i in 1:100
    compute_intensive_task(i)
end
```
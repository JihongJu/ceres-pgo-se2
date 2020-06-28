# ceres-pgo

SE2 Pose Graph Optimization using Ceres-Solver. A copy of [Ceres-Solver's 2D pose graph optimization example](https://github.com/ceres-solver/ceres-solver/tree/master/examples/slam/pose_graph_2d)



## Compile

```sh
mkdir build
cd build
cmake ..
make
```

## Run

```sh
./build/pose_graph_2d --input data/input_M3500_g2o.g2o
```

## Example

![](images/M3500.png)


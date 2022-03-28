# Weighted adjacency matrix of an image
Creates a weighted adjacency matrix from a energy matrix for an image. Average, similarity and dissimilarity between the nodes i,j can be computed. If a custom energy matrix is provided, the same functions can be used to fill the adjacency matrix with edge weights.

# Graphs table
| Type | Images |
| --- | --- |
| 4-noded unidirection | ![fig_4noded_1](https://user-images.githubusercontent.com/28588878/160408425-68133377-68a6-414d-a1fd-862e0ffcbc46.png) |
| 4-noded bidirection | ![fig_4noded_2](https://user-images.githubusercontent.com/28588878/160408470-9e7767aa-7e24-4fa0-ad9b-6ecfa4cc8d2d.png) |
| 8-noded six direction | ![fig_6noded_shortpath](https://user-images.githubusercontent.com/28588878/160408605-0f680020-40c3-4450-9c78-214ca07e458f.png) |
| 8-noded unidirection | ![fig_8noded_1](https://user-images.githubusercontent.com/28588878/160408735-ed4fd455-f0e1-4522-9735-91ad0702f9ae.png) |
| 8-noded bidirection | ![fig_8noded_2](https://user-images.githubusercontent.com/28588878/160408768-3636179c-34ee-4445-87dd-02c434a05e36.png) |

# Requirements
MATLAB <br />

# Run command
Please use the `demo.m` to run the program.

Change the hyper parameters accordingly if needed. But it is not required though.
```
% Inputs
h = 3; w = 6;                       % Image size [height x width]
edgeDirection = 1;                  % Edge direction 1 - uni | 2 - bi
noded = 8;                          % Nodes 4-noded, 6-direction, 8-noded (pixels)
weight_type = 'Average';            % Average (E(i), E(j)) / 2 
                                    % Similarity (E(i) - E(j)) 
                                    % Dissimilarity 1 / (E(i) - E(j)).
                                    % Where E is the energy at node i, j.
```


# Known issues
1. Sometimes `plot(G)` or `plot(G,'Layout','force')` produces strange looking graphs.


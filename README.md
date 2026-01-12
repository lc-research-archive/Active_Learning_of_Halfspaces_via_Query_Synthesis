# Active Learning of Halfspaces via Query Synthesis

This repository contains the MATLAB implementation of the dimension coupling algorithm (DC) for active learning of halfspaces.

## About the Project

This project provides the code for the paper on near-optimal active learning of halfspaces. The algorithm can learn a halfspace in the presence of noise. The core of the implementation is the dimension coupling algorithm (DC) which is a recursive algorithm. It invokes a subroutine `DC2` that couples dimensions.

The implementation was originally for the following paper:
“[Near-Optimal Active Learning of Halfspaces via Query Synthesis in the Noisy Setting](https://arxiv.org/abs/1603.03515)“, in Proc. of 31st AAAI Conference on Artificial Intelligence (AAAI 2017), San Francisco, California, February 2017.

## Getting Started

To run the code, you need to have MATLAB or Octave installed.

### Prerequisites

* MATLAB or Octave

### Usage

1. Clone the repository:
   
   ```sh
   git clone https://github.com/lc-research-archive/Active_Learning_of_Halfspaces_via_Query_Synthesis.git
   ```
2. Open MATLAB or Octave.
3. Run the `main.m` script:
   
   ```matlab
   main
   ```

The script will run the simulation and output the estimated vector, the true vector, the distance between them, and the total number of queries.

## File Descriptions

* `main.m`: The main script that runs the dimension coupling algorithm.
* `DC2.m`: A subroutine invoked by `main.m` that implements the dimension coupling for 2 dimensions.
* `noisy_compute_sign.m`: A function to compute the sign of the dot product with noise.
* `LICENSE`: The license file for the project.
* `README.md`: This file.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

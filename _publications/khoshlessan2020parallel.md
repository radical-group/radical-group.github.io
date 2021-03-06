---
title: "Parallel Performance of Molecular Dynamics Trajectory Analysis"
collection: publications
permalink: /publications/khoshlessan2020parallel
date: 2020-04-27
type: pub
author: "Mahzad Khoshlessan, Ioannis Paraskevakos, Geoffrey C. Fox, Shantenu Jha and Oliver Beckstein"
venue: "Concurrency and Computation: Practise and Experience"
paperurl: https://onlinelibrary.wiley.com/doi/abs/10.1002/cpe.5789
arxiv: https://arxiv.org/abs/1907.00097
abstract: "The performance of biomolecular molecular dynamics simulations has steadily 
increased on modern high performance computing resources but acceleration of the 
analysis of the output trajectories has lagged behind so that analyzing simulations 
is becoming a bottleneck. To close this gap, we studied the performance of parallel 
trajectory analysis with MPI and the Python MDAnalysis library on three different 
XSEDE supercomputers where trajectories were read from a Lustre parallel file 
system. Strong scaling performance was impeded by stragglers, MPI processes that 
were slower than the typical process. Stragglers were less prevalent for 
compute-bound workloads, thus pointing to file reading as a bottleneck for 
scaling. However, a more complicated picture emerged in which both the computation 
and the data ingestion exhibited close to ideal strong scaling behavior whereas 
stragglers were primarily caused by either large MPI communication costs or long 
times to open the single shared trajectory file. We improved overall strong 
scaling performance by either subfiling (splitting the trajectory into separate 
files) or MPI-IO with Parallel HDF5 trajectory files. The parallel HDF5 approach 
resulted in near ideal strong scaling on up to 384 cores (16 nodes), thus 
reducing trajectory analysis times by two orders of magnitude compared to the 
serial approach."
---

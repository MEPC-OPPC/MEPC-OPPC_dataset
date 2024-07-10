# The MEPC-OPPC Dataset
MEPC-OPPC: Synthetic BIM based Occluded Point Cloud Dataset of MEP Components via Realistic LiDAR Simulation

![] (img/Overview2.jpg)

## Abstract

Point clouds are extensively utilized in the Architecture, Engineering, and Construction (AEC) industry for tasks such as factory equipment relocation planning, layout and assembly line planning, global manufacturing operations, 5S and Gemba Walks, best practice sharing, visual interfaces, and Scan-to-BIM processes. An accurate point cloud enhances efficiency and effectiveness in these applications. This paper is utilizing and configuring existing data extraction pipelines for generation, anonymization and alignment of ground truth and partial occluded point cloud data of Mechanical, Electrical, and Plumbing (MEP) components generating and providing pairs of ground truth and occluded point clouds as a coincide dataset. Specifically, a point cloud is generated from detailed Building Information Modeling (BIM) models via simulation of Light Detection and Ranging (LiDAR) output and applying device-specific configuration data from existing commercial devices, replicating the point cloud outcome in reality.  By utilizing the specific labels included in the detailed BIM model data, via point sampling, the ground truth information is being generated in a per-instance fashion, meaning that individual segmented ground truth point clouds of MEP components are created also accompanied by partial counterparts.

## Dataset Discription

The MEPC-OPPC Dataset contains partial occluded and ground truth point clouds of various model types in a MEP environment captured by a real-world based LiDAR simulation. Every file named as e.g., "101145.ply" or "101195.ply" always represents the ground truth point cloud for each object.

## Getting Started

An automatic download script is provided:

```
git clone https://github.com/uulm-mrm/semantic_spray_dataset.git
bash download.sh
```

For the manual download of the data, a guide is also provided [here] (docs/manual_download.md).

## Exploring The Data

The sensor setup used for the simulations is the following:
*Sensors*

   + 2 HESAI XT32M2X 32-Channel Medium-Range Mechanical LiDAR (top- and front-mounted high-resolution LiDAR)

## Visualizing The Data

## Related Work

## Citation

If you find this dataset useful in your research, consider citing our work:

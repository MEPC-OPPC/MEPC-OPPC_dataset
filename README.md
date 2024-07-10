# The MEPC-OPPC Dataset
MEPC-OPPC: Synthetic BIM based Occluded Point Cloud Dataset of MEP Components via Realistic LiDAR Simulation

## Abstract

Point clouds are extensively utilized in the Architecture, Engineering, and Construction (AEC) industry for tasks such as factory equipment relocation planning, layout and assembly line planning, global manufacturing operations, 5S and Gemba Walks, best practice sharing, visual interfaces, and Scan-to-BIM processes. An accurate point cloud enhances efficiency and effectiveness in these applications. This paper is utilizing and configuring existing data extraction pipelines for generation, anonymization and alignment of ground truth and partial occluded point cloud data of Mechanical, Electrical, and Plumbing (MEP) components generating and providing pairs of ground truth and occluded point clouds as a coincide dataset. Specifically, a point cloud is generated from detailed Building Information Modeling (BIM) models via simulation of Light Detection and Ranging (LiDAR) output and applying device-specific configuration data from existing commercial devices, replicating the point cloud outcome in reality.  By utilizing the specific labels included in the detailed BIM model data, via point sampling, the ground truth information is being generated in a per-instance fashion, meaning that individual segmented ground truth point clouds of MEP components are created also accompanied by partial counterparts.

## Dataset Discription

The MEPC-OPPC Dataset contains partial occluded and ground truth point clouds of various model types in a MEP environment captured by a real-world based LiDAR simulation.

## Getting Started

An automatic download script is provided:

```
git clone https://github.com/uulm-mrm/semantic_spray_dataset.git
bash download.sh
```

For the manual download of the data, a guide is also provided (docs/manual_download.md).

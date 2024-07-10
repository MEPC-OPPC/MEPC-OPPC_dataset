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

For the manual download of the data, a guide is also provided [here] (docs/manual_download.md).

## Exploring The Data

The sensor setup used for the recordings is the following:
*Sensors*

   + 1 Front Camera
   + 1 Velodyne VLP32C LiDAR (top-mounted high-resolution LiDAR)
   + 2 Ibeo LUX 2010 LiDAR (front and rear mounted, l.- w-resolution LiDAR)
   + 1 Aptiv ESR 2.5 Radar

*Raw Data*

    + [Camera Image] in the folder "image_2"
    + [VLP32C LiDAR] in the folder "velodyne"
    + [VLIbeo LUX 2010 LiDAR front] in the folder "ibeo_front"
    + [VLIbeo LUX 2010 LiDAR rear] in the folder "ibeo_rear"
    + [Aptiv ESR 2.5 Radar] in the folder "delphi_radar"

*Labels*

    + [Semantic Labels for VLP32C LiDAR] in the folder "labels"
    + [Semantic Labels for Radar] in the folder "radar_labels"
    + [3D Object Labels for VLP32C LiDAR] in the folder "object_labels/lidar"
    + [2D Object Labels for Camera] in the folder "object_labels/camera"

*Misc*

    + The ego vehicle poses are located in the file "poses.txt". The convention used by the SemanticKITTI dataset is followed.
    + Additional information on the scene setup (e.g., ego_velocity) are given in the "metadata.txt" file.

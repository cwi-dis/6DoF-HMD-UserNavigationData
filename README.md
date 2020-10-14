# User Centered Adaptive Streaming of Dynamic Point Clouds with Low Complexity Tiling
In recent years, the development of devices for acquisition and rendering of 3D contents have facilitated the diffusion of immersive virtual reality experiences. In particular, the point cloud representation has emerged as a popular format for volumetric photorealistic reconstructions of dynamic real world objects, due to its simplicity and versatility.
To optimize the delivery of the large amount of data needed to provide these experiences, adaptive streaming over HTTP is a promising solution. In order to ensure the best quality of experience within the bandwidth constraints, adaptive streaming is combined with tiling to optimize the quality of what is being visualized by the user at a given moment; as such, it has been successfully used in the past for omnidirectional contents.
However, its adoption to the point cloud streaming scenario has only been studied to optimize multi-object delivery. 
In this work, we present a low-complexity tiling approach to perform adaptive streaming of point cloud content. Tiles are defined by segmenting each point cloud object in several parts, which are then independently encoded. In order to evaluate the approach, we first collect real navigation paths, obtained through a user study in 6 degrees of freedom with 26 participants. The variation in movements and interaction behaviour among users indicate that a user-centered adaptive delivery could lead to sensible gains in terms of perceived quality. This dataset is made available here for future research. The point cloud dataset used in this work is -

Eugene d’Eon, Bob Harrison, Taos Myers, and Philip A. Chou. 2017.  8i Voxelized Full Bodies - A Voxelized Point Cloud Dataset, ISO/IEC JTC1/SC29 JointWG11/WG1 (MPEG/JPEG) input document WG11M40059/WG1M74006, Geneva.(January 2017)

## User Navigation Dataset
The user navigation dataset was recorded while 26 participants watched 150 looped frames of dynamic point cloud content in the Unity game engine. The location and orientation of their viewport is recorded at every rendered frame. All coordinates are based on the Unity world coordinate system. The XZ plane at the origin represents the floor. The dataset contains the following fields:

(1)  FrameNumber: The frame number for the current point cloud frame being rendered  
(2)  HMDPX: The X coordinate of the viewport  
(3)  HMDPY: The Y coordinate of the viewport  
(4)  HMDPZ: The Z coordinate of the viewport  
(5)  HMDRX: The rotation of the viewport about the X axis  
(6)  HMDRY: The rotation of the viewport about the Y axis  
(7)  HMDRZ: The rotation of the viewport about the Z axis  
(8)  Participant: Identifier for the current participant  
(9)  Dataset: Identifier for the current point cloud sequence  
(10) Viewframe: Frame number in the current session across multiple playback loops  

The datasets numbers refer to the following sequences from the the 8i voxelized full bodies dataset:

(1) H1: Longdress  
(2) H2: Loot  
(3) H3: Red and black  
(4) H4: Soldier  

### We kindly ask that should you mention our dataset in your publication, that you would reference the following paper:

Shishir Subramanyam, Irene Viola, Alan Hanjalic, and Pablo Cesar. User Centered Adaptive Streaming of Dynamic Point Clouds with Low Complexity Tiling. ACM Multimedia (MM 2020), Seatle, United States. October 12-16, 2020

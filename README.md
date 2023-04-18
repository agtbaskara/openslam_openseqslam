OpenSeqSLAM
===========

Copyright 2013, Niko Sünderhauf
Chemnitz University of Technology
niko@etit.tu-chemnitz.de

OpenSeqSLAM is an open source Matlab implementation of the original SeqSLAM
algorithm published by Milford and Wyeth at ICRA12 [1]. SeqSLAM performs place
recognition by matching sequences of images. 

Quick start guide: 
 - Download the Nordland dataset: 
    ```
    cd datasets/norland; ./getDataset.bash;
    ```
 - start Matlab and run demo.m from within the matlab directory


[1] Michael Milford and Gordon F. Wyeth (2012). SeqSLAM: Visual Route-Based Navigation for Sunny Summer Days and Stormy Winter Nights. In Proc. of IEEE Intl. Conf. on Robotics and Automation (ICRA)

# `demo.m` parameter for testing additional datasets:

- carla-sync-wide town02
    ```
    % Reference dataset
    ds.name = 'clearnoon';
    ds.imagePath = '../datasets/carla-sync-wide-gray/town02/clearnoon';
    ...
    ds.imageIndices = 1:ds.imageSkip:793;
    ...
    % Target dataset
        ds.name = 'clearnight';
        ds.imagePath = '../datasets/carla-sync-wide-gray/town02/clearnight';
    ```
- carla-sync-wide town05
    ```
    % Reference dataset
    ds.name = 'clearnoon';
    ds.imagePath = '../datasets/carla-sync-wide-gray/town05/clearnoon';
    ...
    ds.imageIndices = 1:ds.imageSkip:1608;
    ...
    % Target dataset
    ds.name = 'clearnight';
    ds.imagePath = '../datasets/carla-sync-wide-gray/town05/clearnight';
    ```
- tut
    ```
    % Reference dataset
    ds.name = 'day';
    ds.imagePath = '../datasets/tut-gray/tut-backyard/day';
    ...
    ds.imageIndices = 1:ds.imageSkip:607;
    ...
    % Target dataset
    ds.name = 'night';
    ds.imagePath = '../datasets/tut-gray/tut-backyard/night';
    ```
- nordland
    ```
    % Reference dataset
    ds.name = 'summer';
    ds.imagePath = '../datasets/nordland-gray/summer/image_rgb';
    ...
    ds.imageIndices = 22684:ds.imageSkip:28354;
    ...
    % Target dataset
    ds.name = 'winter';
    ds.imagePath = '../datasets/nordland-gray/winter/image_rgb';
    ```
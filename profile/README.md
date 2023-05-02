# SLAM-Hive
**Author**: Yuanyuan Yang, Bowen Xu, Yinjie Li and Sören Schwertfeger


SLAM Hive is a project to enable the systematic, repeatable and reproducable evaluation of SLAM (Simultaneous Localization and Mapping) algorithms. It owns Web graphical user interface, comprehensive evaluation index, user-defined configuration, performance analysis and strong expansibility.

The system is based on Docker container. The use of container technology provides strong expansibility and flexibility for this system. The configuration parameters of mapping tasks and their evaluation results are recorded in the database. Then we can analyze the historical tasks and their corresponding parameter values in detail.

In the future, SLAM-Hive will be deployed to the cluster to explore the broad parameter space of SLAM algorithm. We will also provide a user management system and more evaluation methods and metrics, as well as other follow-up improvements.

<img src="https://github.com/SLAM-Hive/slam_hive_web/blob/main/pictures/Poster.png" width="1620" height="1080" border="10" />

# 1. License
The source code is released under GPLv3 license.

We are still working on improving the code reliability. For any technical issues, you can make an issue.

If you use SLAM-Hive in an academic work, please cite:

    @article{
      title={The SLAM Hive Benchmarking Suite},
      author={Yang, Y., B. Xu, Y. Li, and S. Schwertfeger.},
      conference={Robotics and Automation},
      year={2023}
     }

# 2. How to use
The repositories in project are divided into four parts.

The main part of SLAM-Hive is **slam_hive_web**. You can see the installation help in <https://github.com/SLAM-Hive/slam_hive_web/tree/main>.

The repository <a href="https://github.com/SLAM-Hive/slam_hive_datasets">slam_hive_datasets</a> stores scripts for downloading these different datasets.

The repository <a href="https://github.com/SLAM-Hive/slam_hive_results">slam_hive_results</a> stores the evaluation results which we ran and evaluated when testing.

Other repositories like **orb-slam2-ros-mono** stores the scripts and related files of how to build the algorithm docker image.

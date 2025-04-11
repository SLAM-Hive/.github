# SLAM-Hive
**Author**: Yuanyuan Yang, Bowen Xu, Yinjie Li and Sören Schwertfeger


SLAM Hive is a project to enable the systematic, repeatable and reproducable evaluation of SLAM (Simultaneous Localization and Mapping) algorithms. It owns Web graphical user interface, comprehensive evaluation index, user-defined configuration, performance analysis and strong expansibility.

The system is based on Docker container. The use of container technology provides strong expansibility and flexibility for this system. The configuration parameters of mapping tasks and their evaluation results are recorded in the database. Then we can analyze the historical tasks and their corresponding parameter values in detail.

We are working on enable SLAM-Hive to be deployed to clusters to explore the broad parameter space of SLAM algorithms. We will also provide a user management system and more evaluation methods and metrics, as well as other follow-up improvements.

<img src="https://github.com/SLAM-Hive/slam_hive_web/blob/main/pictures/ICRA2023_Poster.png"  border="10" />

The paper was published at the 2023 IEEE international conference on robotics and automation (ICRA) and is available on arxiv: <a href="https://arxiv.org/abs/2303.11854">here</a>

Also 2024 Journal preprint (arXiv PDF): <a href="https://arxiv.org/abs/2406.17586">here</a>

# 1. License
The source code is released under [GPLv3](http://www.gnu.org/licenses/) license.

We are still working on improving the code reliability. For any technical issues, you can make an issue.

If you use SLAM-Hive in an academic work, please cite:

Yang, Yaxun, Bowen Xu, Yinjie Li, and Sören Schwertfeger,  "The SLAM Hive Benchmarking Suite",  Robotics and Automation (ICRA), 2023 IEEE International Conference on, 2023.

    @inproceedings{
      title={The SLAM Hive Benchmarking Suite},
      author={Yang, Yuanyuan and Xu, Bowen and Li, Yinjie and Schwertfeger, S{\"o}ren},
      booktitle={2023 IEEE international conference on robotics and automation (ICRA)},
      year={2023}
     }
2024 Journal preprint (arXiv PDF): 

    @misc{liu2024benchmarkingslamalgorithmscloud,
          title={Benchmarking SLAM Algorithms in the Cloud: The SLAM Hive Benchmarking Suite}, 
          author={Xinzhe Liu and Yuanyuan Yang and Bowen Xu and Delin Feng and Sören Schwertfeger},
          year={2024},
          eprint={2406.17586},
          archivePrefix={arXiv},
          primaryClass={cs.RO},
          url={https://arxiv.org/abs/2406.17586}, 
    }

# 2. How to use
The repositories in project are divided into four parts.

The main part of SLAM-Hive is **slam_hive_web**. You can see the installation help in <https://github.com/SLAM-Hive/slam_hive_web/tree/main>.

The repository <a href="https://github.com/SLAM-Hive/slam_hive_datasets">slam_hive_datasets</a> stores scripts for downloading these different datasets.

The repository <a href="https://github.com/SLAM-Hive/slam_hive_results">slam_hive_results</a> stores the evaluation results which we ran and evaluated when testing.

Other repositories like **orb-slam2-ros-mono** stores the scripts and related files of how to build the algorithm docker image.

# 3. SLAM-Hive repo overview

Our group contains some repos, mainly about:
 - slam_hive_web
	 -  The website repo. We introduce the code details in <https://github.com/SLAM-Hive/slam_hive_web/blob/main/README.md>.
 - slam_hive_controller
	 - This is a middle controller module of SLAM Hive, using mainly in cluster and aliyun modes. This module is also used for dataset pre-processing. We introduce the code details in <https://github.com/SLAM-Hive/slam_hive_controller/blob/main/README.md>.
 - algorithms
	 - Group has many algorithm containers repo, for example: orb-slam2-ros-mono；Each repo can be used to build an image 
 - slam_hive_datasets
	 -  In slam_hive_datasets, we offer the dataset downloading script and rorbag replay script for each supported dataset.
 - slam_hive_results
	 - This repo has our ICRA 2023 experiments; Our journal paper experiments can be downloaded at <http://robotics.shanghaitech.edu.cn/static/datasets/SLAM-Hive/SLAM-Hive_archive.zip>

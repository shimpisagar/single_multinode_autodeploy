# cloud_hdp_auto_deploy
HDP automated install using blueprint

This code will help you to install Ambari along with HDP in automated way irrespective of on-premises or cloud environment.

#+++++++++++++++++++++++++

#setup_cluster.sh - This is parent script. Running this script along with arguments set up your HDP cluster in automated way. Before you run this script make sure you have modified "cluster_props" file according to your environment.
	
#cluster.props - This script is used when you are installing hadoop ON_PREMISES or Bare-Metal servers. This file defines variables used to install/setup Ambari and HDP. Please do make sure you have set correct values in this file.

#cluster_cloud.props - For Cloud installation you need to provide this file as params to "setup_cluster.sh" script.This file defines variables used to install/setup Ambari and HDP. Please do make sure you have set correct values in this file.

#generate_json.sh - This will generate blueprint and trigger the HDP installation.

#post_script.sh - Post script will execute add-on task required to be setup after HDP installation.

#+++++++++++++++++++++++++


#=========================
#Steps run the script
#=========================

#git clone https://github.com/shimpisagar/single_multinode_autodeploy.git

#./setup_cluster.sh <path_to_cluster_props_file>

# -------------- ndt_mapping ------------------------#
Node [/points_map_loader]
Publications: 
 * /pmap_stat [std_msgs/Bool]
 * /rosout [rosgraph_msgs/Log]
 * /points_map [sensor_msgs/PointCloud2]	// This is the map data which displays on Rviz.

Subscriptions: None

Services: 
 * /points_map_loader/set_logger_level
 * /points_map_loader/get_loggers


contacting node http://maitereo-Surface-Book:41980/ ...
Pid: 4885
Connections:
 * topic: /rosout
    * to: /rosout
    * direction: outbound
    * transport: TCPROS
 * topic: /points_map
    * to: /rviz_1536747554370633532
    * direction: outbound
    * transport: TCPROS
 * topic: /pmap_stat
    * to: /runime_manager_3733_1536747327591
    * direction: outbound
    * transport: TCPROS

//=========== sensor_msgs/PointCloud2 ==========//

{/points_map & /points_raw} // topics which use the msg

std_msgs/Header header
  uint32 seq
  time stamp
  string frame_id
uint32 height		// height of resolution
uint32 width		// width of resolution
sensor_msgs/PointField[] fields
  uint8 INT8=1
  uint8 UINT8=2
  uint8 INT16=3
  uint8 UINT16=4
  uint8 INT32=5
  uint8 UINT32=6
  uint8 FLOAT32=7
  uint8 FLOAT64=8
  string name
  uint32 offset
  uint8 datatype
  uint32 count
bool is_bigendian
uint32 point_step
uint32 row_step
uint8[] data
bool is_dense
//===============================================//

# ------------------------------------------------#


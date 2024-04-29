# BUGREVIEW
review my bug


. 2024.4.28-4.29  gazebo 不发布TF数据
 .. launch 文件确实状态发布标签。
 <!-- run joint_state_publisher node，publish joint state   -->
    <node name="joint_state_publisher" pkg="joint_state_publisher" type="joint_state_publisher" ></node> 

    <!-- run robot_state_publisher node，pubish tf  -->
    <node name="robot_state_publisher" pkg="robot_state_publisher" type="robot_state_publisher"  output="screen" >
        <param name="publish_frequency" type="double" value="50.0" />
    </node>

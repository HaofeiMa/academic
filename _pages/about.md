---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

I am now a master student in the [National Key Laboratory of Robot Technology and Systems](http://robot.hit.edu.cn/) of [Harbin Institute of Technology](https://www.hit.edu.cn/), mainly engaged in the research of robot autonomous operation technology based on pose estimation and imitation learning.

I graduated from [School of Mechanical Engineering](https://mes.hebut.edu.cn/), Hebei University of Technology (河北工业大学机械工程学院) with a bachelor’s degree。 Now, I'm pursuing my master’s degree in the [School of Mechatronics Engineering](http://sme.hit.edu.cn/), Harbin Institute of Technology (哈尔滨工业大学机电工程学院), advised by Weidong Wang ([王伟东](http://homepage.hit.edu.cn/wangweidong)).

My research interest includes robot operation, grasping, object pose estimation. I have submitted 5 papers in SCI journals, applied 1 invention patent, authorized 3 utility model patents and 1 software copyright.



<!-- 
# 🔥 News
- *2022.02*: &nbsp;🎉🎉 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2022.02*: &nbsp;🎉🎉 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
-->

# 📖 Educations
- *2022.09 - 2024.06 (now)*, [Harbin Institute of Technology](https://www.hit.edu.cn/), Harbin, (Percentage: 90.65, rank: 5/112).
- *2018.09 - 2022.06*, [Hebei University of Technology](https://www.hebut.edu.cn/), Tianjin, (CGPA: 3.95/4, rank: 1/133).


# 🔍 Projects

<!-- Project -->

## Sampling Robots in Complex Environments

<div class='paper-box'>
<div class='paper-box-image'>
<div class="badge">2023.03 - Present</div>
<img src='images/202303_Sampling_Robots_in_Complex_Environments.png' alt="sym" width="100%">
</div>
<div class='paper-box-text' markdown="1">

Because of the irregularities on the object's surface and variations in lighting conditions, point cloud images obtained from a single perspective often contain significant gaps and errors at the object's edges, which can lead to inaccurate grasping pose estimations. To tackle these challenges, this article proposes a practical robot grasping method based on 6D pose estimation and point cloud fusion. First, 6D pose estimation is conducted, utilizing the results from model point cloud and pose estimation to complete the input point cloud through ICP (Iterative Closest Point). Subsequently, the resulting complete object point cloud is used to estimate the 6D grasping pose of the object with the help of the grasping direction estimation network.

</div><div markdown="1">

**Finished Works**:
1. Establish a model-free 6D pose estimation network based on perspective matching. Construct and train the pose estimation network to achieve precise pose estimation for seen objects and a rough estimation method for untrained objects. Create a pose refinement network for untrained objects when sparse point clouds are accessible.

2. Propose a point cloud fusion and filtering method based on pose estimation. This method addresses the issue of point cloud gaps at the edge of objects when the robot collects samples from a single perspective. The point cloud fusion method is designed to utilize the output of pose estimation to fill in the gaps in the input point cloud and remove noise.

3. Perform grasp pose estimation using the completed point cloud. Utilizing the grasping angle prediction network and a fast search strategy, the completed point cloud enhances the stability of grasping pose generation, thereby improving the success rate of grasping and its robustness.

4. Test the system in simulation and the real world using a 6DoF robot, a Realsense camera, and a laptop (ROS/Ubuntu 20.04) as the host computer.

</div>
</div>

<!-- Project -->

## Autonomous Suture Robot System for Endoscopic Surgery

<div class='paper-box'>
<div class='paper-box-image'>
<div class="badge">2023.02 - 2023.07</div>
<img src='images/202302_Autonomous_Suture_Operation_Robot_System_for_Endoscopic_Surgery.png' alt="sym" width="100%">
</div>
<div class='paper-box-text' markdown="1">

The research objective is to enhance the efficiency and accuracy of autonomous suturing in endoscopic surgery. This involves designing a 3DOF autonomous suturing instrument, developing an efficient laparoscopic surgery robot based on 3D laparoscopy, and establishing a robot system that integrates visual, expert, and navigation systems.

</div><div markdown="1">

**Finished Works**:
1. Perform the recognition and segmentation of surgical instruments and lesion tissues based on Yolov8, and determine the spatial position of the end of the surgical instruments.

2. Build a vision and robotic arm fusion system, perform hand-eye calibration of cameras and robotic arms, and execute basic robot actions for visual servo.

</div>
</div>

<!-- Project -->

## Rock Core Box Handling Robot

<div class='paper-box'>
<div class='paper-box-image'>
<div class="badge">2022.08 - 2023.02</div>
<img src='images/202208_Rock_Core_Box_Handling_Robot.jpg' alt="sym" width="100%">
</div>
<div class='paper-box-text' markdown="1">

Rock Core samples obtained from drilling before oil extraction are crucial data for assessing mining value, and they are stored in dedicated core boxes. During research and analysis, it's essential to arrange these rock core boxes neatly on-site in a designated order, one box at a time. However, these boxes are typically heavy, resulting in a high labor intensity that can impact transportation efficiency. The present invention aims to address the labor intensity associated with the current method of transporting core boxes, ultimately improving transportation efficiency.

</div><div markdown="1">

**Finished Works**:
1. Build a sensing system that utilizes infrared sensors to detect surrounding obstacles, as well as fractional laser sensors to detect the current stacking height and alignment.

2. Implement rock core box instance segmentation based on Mask RCNN, combined with a depth camera to determine its corner space coordinates for visual servo during the robot handling process.

3. Utilize a monocular camera and Aruco markers to achieve 2D pose adjustment of the robot in place by identifying the offset distance and angle of the Aruco marker.

</div>
</div>

<!-- Project -->

## Medical Pan-Tilt Control System Based on Binocular Vision

<div class='paper-box'>
<div class='paper-box-image'>
<div class="badge">2022.01 - 2022.06</div>
<img src='images/202201_Medical_Multi-DoF_Pan-Tilt_Control_System_Based_on_Binocular_Vision.jpg' alt="sym" width="100%">
</div>
<div class='paper-box-text' markdown="1">

In traditional medical processes, traditional Chinese medicine practitioners often need to frequently change positions and adjust their angles to view the surgical area. Additionally, during rehabilitation treatment, the camera's range can be inadequate to cover the patient's moving area. Current recording methods commonly used suffer from limitations and lack automation. This article introduces a multi-degree-of-freedom pan-tilt system designed to track the positions of doctors and patients.

[**Project**](https://github.com/HaofeiMa/Multi-DOF_PTZ), [**Video**](https://www.youtube.com/watch?v=gDLijtdpC2w)

</div><div markdown="1">

**Finished Works**:
1. Design the mechanical structure and simulate the platform's motion, using internal toothed rotary bearings to minimize the structural size. Protective structures have been designed for all sensor components.

2. Design hardware control algorithms for pan-tilt using STM32 and A4988 drivers, and establish communication between STM32 and the host computer's ROS system for pan-tilt motion control within ROS.

3. Propose a target tracking method based on HOG and SIFT feature matching, capable of short-term single target tracking while maintaining robustness to changes in the target object's appearance.

4. Construct an experimental Pan-Tilt system and conduct experiments with all proposed algorithms, using 3D printed structural components, a Realsense camera, and stepper motors.

</div>
</div>

<!-- Project -->

## Spherical Environmental Information Collection Robot

<div class='paper-box'>
<div class='paper-box-image'>
<div class="badge">2020.11 - 2021.05</div>
<img src='images/202011_Spherical_Metamorphic_Environmental_Information_Collection_Robot.gif' alt="sym" width="50%">
<img src='images/202011_Spherical_Metamorphic_Environmental_Information_Collection_Robot.png' alt="sym" width="50%">
</div>
<div class='paper-box-text' markdown="1">

Monitoring essential information in various hazardous environments, such as petrochemical plants, chemical plants, and disaster sites, is vital for disaster prevention and reduction. In response to this need, our team has designed a spherical environment monitoring robot system. It features a spherical metamorphic structure with multiple telescopic feet that enable the robot to rotate, roll, and achieve all-round motion with high stability. These robots utilize self-organized network communication technology to offer multiple monitoring modes, and the collected data is packaged and transmitted to the upper computer system, enabling real-time dynamic monitoring of complex environmental information over a wide area.

</div><div markdown="1">

**Finished Works**:
1. Design the three-dimensional structure of the spherical robot, including the placement of controllers, sensors inside the sphere, and the spatial arrangement of leg motors.
2. Implement control of spherical robot leg motors using STM32, calculate motion strategies, and achieve robot motion.
3. Integrate , accelerometers, temperature and humidity sensors, gas sensors, etc., into the STM32 control system for Bluetooth-controlled robot motion and sensor data reception.

</div>
</div>

# 📝 Publications 

## 📃 Papers

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Robotics and Autonomous Systems</div><img src='images/202309_A_study_of_robotic_search_strategy_for_multi-radiation_sources_in_unknown_environments.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[A study of robotic search strategy for multi-radiation sources in unknown environments](https://doi.org/10.1016/j.robot.2023.104529)

Hua Bai, Wenrui Gao, **Haofei Ma**, Pengchao Ding, Gongcheng Wang, Wenda Xu, Weidong Wang, Zhijiang Du

[**Paper**](https://doi.org/10.1016/j.robot.2023.104529)
- A robot search strategy is proposed and evaluated for unknown radiation environments.
- Combine ADE optimization with the PSPF algorithm to improve estimation efficiency.
- An exploration scheme is proposed to balance exploration and exploitation.

</div>
</div>

<!--
[**Project**](https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=DhtAFkwAAAAJ&citation_for_view=DhtAFkwAAAAJ:ALROH1vI_8AC) <strong><span class='show_paper_citations' data='DhtAFkwAAAAJ:ALROH1vI_8AC'></span></strong>
- Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
</div>
</div>

- [Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet](https://github.com), A, B, C, **CVPR 2020**
-->

- <code class="language-plaintext highlighter-rouge">Robotics and Autonomous Systems</code> [**Robotic Grasping Method with 6D Pose Estimation and Point Cloud Fusion**](https://www.sciencedirect.com/journal/robotics-and-autonomous-systems), **Haofei Ma**, Gongcheng Wang, Hua Bai, Zhiyu Xia, Weidong Wang, Zhijiang Du (Under Review)

- <code class="language-plaintext highlighter-rouge">Robotics and Autonomous Systems</code> [**Reactive Mobile Manipulation Based on Dynamic Dual-Trajectory Tracking**](https://www.sciencedirect.com/journal/robotics-and-autonomous-systems), Gongcheng Wang, **Haofei Ma**, Han Wang, Pengchao Din,g Hua Bai Wenda Xu, Weidong Wang, Zhijiang Du (Under Review with Revisions Submitted)

- <code class="language-plaintext highlighter-rouge">Robotics and Automation Letters</code> [**Dynamic Planning of Mobile Manipulator Based on Perception Prediction**](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=7083369), Gongcheng Wang, Han Wang, **Haofei Ma**, Wenda Xu, Pengchao Ding, Hua Bai, Weidong Wang, Zhijiang Du(Under Review)

- <code class="language-plaintext highlighter-rouge">IEEE Sensors Journal</code> [**Kalman Filter-based EM-optical Sensor Fusion for Bone Needle Position Tracking**](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=7361), Zhiyu Xia, Han Wang, Yulong Men, **Haofei Ma**, Zexin Cao, Weidong Wang, Zhijiang Du (Under Review with Revisions Submitted)

## 📚 Patents

- <code class="language-plaintext highlighter-rouge">Invention Patent</code> [**A Rock Core Box Handling Robot**](https://cprs.patentstar.com.cn/Search/Detail?ANE=9DIE1BAA2AAA8CDA8EDA9CIB9BIF9GBC9BED6BDA9HBH9IBE), Weidong Wang, Hengbin Liang, **Haofei Ma**, Gongcheng Wang (CN202310547284.5, Pending)

- <code class="language-plaintext highlighter-rouge">Utility Model Patent</code> [**A Spherical Metamorphic Robot and An Environmental Information Monitoring System**](https://cprs.patentstar.com.cn/Search/Detail?ANE=AHIA8FDA8AGA9GGE9HAA6GAA9HDD9CIC9FCA9HDC9GDF9ICF), Yuhan Rao, Manhong Li, *Haofei Ma*, Yuchong Gao, Nuo Zhang, Xinyu Liu (CN202120212154.2)

- <code class="language-plaintext highlighter-rouge">Utility Model Patent</code> [**A Rope Driven Cleaning Robot**](https://cprs.patentstar.com.cn/Search/Detail?ANE=AIHA6AGA7BEA9DID9BIC9ICBBFIA8BDA9IBF9ICG8EEA9FDG), Bao Li, Manhong Li, Shuofan Li, **Haofei Ma**, Jidong Guo, Yuchong Gao, Yingxin Dong (CN202120545507.0)

- <code class="language-plaintext highlighter-rouge">Utility Model Patent</code> [**Small Ocean Vehicles Using Wave Energy to Generate Electricity**](https://cprs.patentstar.com.cn/Search/Detail?ANE=9EEB9HFD3ABA3CBA9AIB9GIF8IAA9FADBCIA9BEA9ECDAGGA), Yihan Gao, **Haofei Ma**, Shaoan Chen, Haoran Sun, Chenxi Song (CN202020078465.X)

- <code class="language-plaintext highlighter-rouge">Software Copyright</code> **Identity Recognition and Infrared Temperature Measurement Control System**, **Haofei Ma** (2021SR1391064)

# 🏆 Honors and Awards

## 🏅 Honors
- *2023.09*, Top Grade Scholarship in Harbin Institute of Technology
- *2022.06*, Provincial Outstanding Graduates (Top 1%)
- *2021.05*, Provincial Merit Student (Top 1%)
- *2021.06*, Finely Crafted Technology Scholarship
- *2021.01*, Outstanding Student in Hebei University of Technology
- *2020.12*, [National Scholarship](https://mp.weixin.qq.com/s/ulEa10HIwbCN9yk4mXRcVQ) (Top 0.3%)
- *2020.12*, Excellent Student Cadre in Hebei University of Technology
- *2020.12*, The First Prize Scholarship in Hebei University of Technology

## 🎏 Competitions
- *2021.09*, “Internet +” Innovation and Entrepreneurship Competition Provincial Silver Award .
- *2021.08*, E-commerce “Innovation, Creativity, and Entrepreneurship” Challenge Provincial Third Prize.
- *2021.07*, Zhou Peiyuan Mechanics Competition Provincial Second Prize and National Excellence Award.
- *2020.12*, Hebei Province College Robot Competition Seconda Prize.
- *2020.10*, Electronic Design Competition Provincial Second Prize.
- *2020.10*, iCAN International Innovation and Entrepreneurship Competition Provincial Second Prize.
- *2020.09*, Mechanical Innovation Design Competition Provincial Second Prize.
- *2019.12*, Mathematics Competition Provincial First Prize.
- *2019.09*, iCAN International Innovation and Entrepreneurship Competition Provincial Third Prize.
- *2019.06*, Mathematics Competition Provincial Second Prize.

# 💼 Societies

- *2023.02 - 2023.07*, School Office Assistant in Harbin Institute of Technology.
- *2022.02 - 2022.06*, Class Leader in Hebei University of Technology.
- *2019.09 - 2022.06*, Class Study Monitor in Hebei University of Technology.
- *2020.09 - 2021.08*, Director of Haier Key Maker-Lab in Hebei University of Technology.

<!-- 
# 💬 Invited Talks
- *2021.06*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2021.03*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet.  \| [\[video\]](https://github.com/)
-->

<!-- 
# 💻 Internships
- *2019.05 - 2020.02*, [Lorem](https://github.com/), China.
-->
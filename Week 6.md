---
layout: page
title: Blogging Like a Hacker
permalink: /Week 6
---
 <!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="description" content="wangzhaogui's page,let u know me" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <style>
        body {
            padding: 10px 0;
        }
    </style>
    <title>Week 6 (25 September - 1 October)</title>
</head>
<body>
     <div class="info-wrap">
      <div class="img">
        <img src="https://z1.ax1x.com/2023/09/28/pPbfSmR.png" alt="">
      </div>
      <div class="info-right">
    <h1>Diver work</h1>
  
    <dl>
        <dt>Sixth Week Schedule</dt>
        <dd>The group held a meeting at 1:30 p.m. on 28 September. This week we optimized the details of the project design and discussed each section with our mentor. 


<dd>
1. ** Opening Equipment: **

The main motion of the tool is the rotation of the milling cutter and the feed motion is perpendicular to the cutting surface downwards. In response to the tool's need for a motion pattern, I plan to use a ball screw to fulfill this need. Ball screws convert rotary motion into linear motion with low friction loss and high transmission efficiency. The spindle is powered by a power source to rotate the tool to accomplish the main motion. The spindle is connected to the inner ring of the ball bearing and the nut of the ball screw is connected to the outer ring of the bearing so that the rotation of the spindle does not affect the movement of the nut. The ball screw is powered from another power source to move the nut downward to complete the feed.
<div class="img">
        <img src="https://z1.ax1x.com/2023/09/28/pPbWJdx.png" alt="">
      </div>
<dd>
2. ** Robotic Arm End-effector**

The opening and closing of the end effector is driven by the motor, and the movement of the end effector is controlled by the manipulator. 
A thin film pressure sensor FSR402 is embedded in the finger belly to detect the clamping force when the end-effector is closed. 
The FSR402 is a resistive pressure sensor. It is allowed to be used in the occasion of pressure 100g-10kg. It can be used to detect the end of the mechanical gripper.
<dd>
Materials required: 
<dd>
Arduino Uno Development board *1
<dd>
Breadboard *1
<dd>
FSR 402 Force resistor *1 
<dd>
LED *110k Ohm and 220 Ohm resistance *1
<dd>
FSR402 principle formula:
<dd>
Vo = Vcc*(R/R+FSR)
<dd>
FSR402 parameters:
<dd>
1. Working voltage: 5VDC@165mA;
<dd>
2. Sensor sensing area: 12.7mm;
<dd>
3. Sensor induction type: passive variable resistance;
<div class="img">
        <img src="https://z1.ax1x.com/2023/09/28/pPbW7T0.png" alt="">
      </div>


<dd>
3. **Analysis of motion planning of mechanical arm **
The design of the robot base has an important influence on motion planning and work stability. This section introduces the design principles and common types of robotic arm bases and discusses their role in motion planning. The design of the manipulator base is an important part of the manipulator motion planning, and its design is designed to provide a stable support and moving platform. When designing the base, structural rigidity needs to be considered: the base should have sufficient structural rigidity to withstand the weight of the robotic arm and the inertia force generated during the movement, so as to ensure the stability and accuracy of the robotic arm in the work. It is preliminarily envisaged that the steel frame structure of the robot base is mainly composed of different types of I-beam and box steel, and the material selected for the robot base structure is Q235A steel, the yield stress of Q235A steel is 235MPa, the Young's elastic modulus is 2.1e11Pa, the Poisson's ratio is 0.3, and the density is 7850kg/m3.

<div class="img">
        <img src="https://z1.ax1x.com/2023/09/28/pPbWhlQ.png" alt="">
      </div>


<dd>
4. **Profile Design **
The first is the force exerted at rest and the second is the extra horizontal inertial force during motion. 
At rest in the vertical direction, in order to keep the mechanical arm at a level of stability and immobility, should be in the vertical direction of the seabed on the mechanical arm of the support force is equal to gravity minus buoyancy, horizontal on the level of the horizontal dragging force will be oscillatory impact on the mechanical arm, the level of the speed is sometimes positive and sometimes negative, and therefore the drag force on the column is also sometimes positive and sometimes negative; its Morrison equation for the fd and the Morrison equation for the horizontal inertial force is f

<div class="img">
        <img src="https://z1.ax1x.com/2023/09/28/pPbWlQJ.png" alt="">
      </div>

<dd>
5. **Equipment Automation**

The working principle of the hydraulic system is as follows: when the gate needs to be opened, the oil is fed into the system by the hydraulic pump and enters the rodless cavity of the hydraulic cylinder through the electro-hydraulic proportional reversing valve right position, one-way throttle valve, balancing circuit and speed control valve. The hydraulic fluid pushes the hydraulic rod outward, and through the expansion of the connecting rod to drive the rotation of the door leaf to open and reach the specified position. The gate closure situation is similar, it will not be repeated. 
The Pressurized Hole Opener uses a scale to measure the feed stroke, and the scale screw mechanism drives the scale bar through the screw nut to mark the hole opening process. Scale bar is equipped with three bumpers, you can move the bumpers in the preset distance after the fixed, when the scale bar movement to the pre-set position, the bumpers will collide with the cam in the hydraulic control valve block, the hydraulic system will immediately carry out the conversion of different working conditions, Figure 2 for the hydraulic control system of the hole opener diagram.


<div class="img">
        <img src="https://z1.ax1x.com/2023/09/28/pPbWqYT.png" alt="">
      </div>


<dd>

    </dl>
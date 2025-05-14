---
layout: project
title: Custom 3D Printed Cycloidal Gearbox
description: Cornell Mars Rover Arm Actuators Project
technologies: [Autodesk Inventor, ANSYS]
image: /assets/images/IMG_6990.jpg
---

Project Overview: 

As a member of the arm subteam on Cornell Mars Rover, I've been designing and manufacturing custom cycloidal gearboxes in order to move away from using off-the-shelf Laiful Harmonics.Due to the size constraints of the arm, classic gearboxes are not viable and the only possible types are Harmonic, Cycloidal, and Planetary. I decided to focus on cycloidals as they don't require any hard to obtain materials (i.e. flex spline in harmonics) and are very robust. I also decided to first focus on a simpler 3D printed prototype so that I could gain a better understanding of these complex systems. 

Preliminary Calculations:

I performed preliminary analysis to determine important metrics of the gearbox, such as determining that a 18:1 ratio would allow for the motors to run at only 50% of stall torque in the max load case. I also determined the dimensions of cycloidal rotor by using equation driven sketches with the following parametric equations

X = (75*cos(t))-(11.25*cos(t+atan(sin((1-75)*t)/((75/(5.625*75))-cos((1-75)*t)))))-(5.625*cos(75*t))

Y = (-75*sin(t))+(11.25*sin(t+atan(sin((1-75)*t)/((75/(5.625*75))-cos((1-75)*t)))))+(5.625*sin(75*t))

Design:

For this design, I mostly stuck to the most basic version of a cycloidal, making all part
geometries optimized for running smoothly. The 4 main parts are the input shaft which is
supported by 3 bearings, the rotor gear which has an epitrochoidal shape, the output shaft which
interfaces with the input at a small bearing to provide stability, and the case which has 19 rollers
corresponding to an 18:1 GR. 

Manufacturing and Testing:

The gearbox was very easy to manufacture as it was made up of 3D printed parts and MCMASTER parts. Assembly went smoothly and I was able to test important gearbox metrics:

Static efficiency: 66%
Backlash 34 arcmin






Aenean faucibus luctus est, sed bibendum tellus. Nulla et magna urna. Morbi a ipsum sollicitudin, rhoncus risus volutpat, ultricies nunc. Quisque mollis finibus ante id imperdiet. Quisque vehicula elit sit amet felis facilisis fermentum.


This is how I solved the problem:

```python
    some code = 10;
    plot();
```

Aenean tincidunt aliquam arcu, in euismod dui dapibus eu. In placerat, mi et ultrices consequat, quam ligula cursus mauris, in semper neque nibh at est. Maecenas hendrerit dignissim porta. Phasellus nec fringilla dolor. Etiam efficitur nisi sit amet velit pharetra feugiat. Etiam ultrices turpis at leo semper, eleifend scelerisque neque malesuada. Aliquam molestie congue rhoncus. Donec blandit neque dolor, nec tristique mi pretium ac. Mauris tincidunt ullamcorper magna, nec pellentesque mi sagittis quis.



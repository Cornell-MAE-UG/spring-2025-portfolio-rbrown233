---
layout: project
title: 3D Printed Cycloidal Gearbox
description: Cornell Mars Rover Arm Actuators Project
technologies: [Autodesk Inventor, ANSYS]
image: /assets/images/IMG_6990.jpg
order: 1
---

Project Overview: 

As a member of the arm subteam on Cornell Mars Rover, I've been designing and manufacturing custom cycloidal gearboxes in order to move away from using off-the-shelf Laiful Harmonics.Due to the size constraints of the arm, classic gearboxes are not viable and the only possible types are Harmonic, Cycloidal, and Planetary. I decided to focus on cycloidals as they don't require any hard to obtain materials (i.e. flex spline in harmonics) and are very robust. I also decided to first focus on a simpler 3D printed prototype so that I could gain a better understanding of these complex systems. 

Preliminary Calculations:

I performed preliminary analysis to determine important metrics of the gearbox, such as determining that a 18:1 ratio would allow for the motors to run at only 50% of stall torque in the max load case. I also determined the dimensions of cycloidal rotor by using equation driven sketches with the following parametric equations

X = (75*cos(t))-(11.25*cos(t+atan(sin((1-75)*t)/((75/(5.625*75))-cos((1-75)*t)))))-(5.625*cos(75*t))

Y = (-75*sin(t))+(11.25*sin(t+atan(sin((1-75)*t)/((75/(5.625*75))-cos((1-75)*t)))))+(5.625*sin(75*t))

![Photo of CAD]({{ "/assets/images/Screenshot 2025-05-13 212023.png" | relative_url }}){: .inline-image-l}

![Photo of Gearbox]({{ "/assets/images/spin.gif" width="150" | relative_url }}){: .inline-image-r}
Design:

For this design, I mostly stuck to the most basic version of a cycloidal, making all part
geometries optimized for running smoothly. The 4 main parts are the input shaft which is
supported by 3 bearings, the rotor gear which has an epitrochoidal shape, the output shaft which
interfaces with the input at a small bearing to provide stability, and the case which has 19 rollers
corresponding to an 18:1 GR. Once the design was finalized, I performed ANSYS strucutural analysis on the case, checking the max bending moment that would be applied if it was being used on the arm.

![Photo of CAD]({{ "/assets/images/ansys.png" | relative_url }}){: .inline-image-l}


Manufacturing and Testing:


The gearbox was easy to manufacture as it was made up of 3D printed parts and MCMASTER parts.I was able to test important gearbox metrics by driving the gearbox with a Maxon Brushless DC motor and Moteus encoder:

Static efficiency: 73%. 
Backlash: 34 arcmin. 
Backdriveable under reasoable amount of force, and no parts failed under 2/3 max torque load.










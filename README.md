pydmps
======

This is a fork of the python library pydmps developed by Mr. Travis DeWolf (aka studywolf). The reason for this fork is that we wanted to apply his nice library to robotics applications, and for that we needed small modifications. More specifically, we needed that the generated trajectories did not mirror in the z-axis. For example, in a pick-and-place task, we want the robot to always move from one place to another following an upward arch, never a downard arch. So we customized the scaling factor to eliminate the mirroring.

For more details about this adaptation, take a look at this paper, subsection II.C., equations 6 and 7:

Pastor, P., Hoffmann, H., Asfour, T. and Schaal, S., 2009, May. Learning and generalization of motor skills by learning from demonstration. In 2009 IEEE International Conference on Robotics and Automation (pp. 763-768). IEEE. (https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=5152385)

Below you will find the text of the original README from Mr. DeWolf:

Dynamic movement primitives (DMPs) are a method of trajectory control / planning from Stefan Schaal’s lab. They were presented way back in 2002 in this paper (http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.142.3886), and then updated in 2013 by Auke Ijspeert in this paper (http://www-clmc.usc.edu/publications/I/ijspeert-NC2013.pdf). This work was motivated by the desire to find a way to represent complex motor actions that can be flexibly adjusted without manual parameter tuning or having to worry about instability.

This repository is a Python implementation of DMPs, with accompanying tutorials and applications that can be found at http://studywolf.wordpress.com/category/robotics/dynamic-movement-primitive/

All that's required for the installation and running of the code is ```numpy```. To run the test code you will also need ```matplotlib``` for displaying the results.


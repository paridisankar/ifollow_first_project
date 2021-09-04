# ifollow_first_project
Executing commands			
			
	Execution for the first time		
		roscore &	
			
	Open 2 terminals: one for the publisher, another one for the subscriber		
		cd my_first_package	
		catkin_make	
		source devel/setup.bash	
			
	Executions of Publisher/Subscriber combinations		
		[frenquency rate] are set amoung this list [10; 20; 50; 100; 200; 500]	
	a		
		Terminal 1	rosrun my_first_package listener
		Terminal 2	rosrun my_first_package talker.py [frenquency rate]
	b		
		Terminal 1	rosrun my_first_package listener
		Terminal 2	rosrun my_first_package talker [frenquency rate]
	c		
		Terminal 1	rosrun my_first_package listener.py
		Terminal 2	rosrun my_first_package talker.py [frenquency rate]
	d		
		Terminal 1	rosrun my_first_package listener.py
		Terminal 2	rosrun my_first_package talker [frenquency rate]

Question 1.	
	ROS C++ is faster than ROS python which has been demonstrated below.
	
Question 1. A.	
	As analyzed in the “ROS publisher-subscriber performance.xslx” file, the measured values are different from the real values for publisher frequency rates above 100 Hz.
	
Question 1. B.	
	The performance difference of different Publisher/Subscriber combinations are commented in “ROS publisher-subscriber performance.xslx” file.
	
Question 1. C.	
	roscpp is a library written in C++ which is a low level language thus it performs better as the executing code is compiled into binary code.
	rospy is a library written in Python which is a high lev

#           MOBILE ROBOTICS

## PDE4430_COURSE WORK 2

## Objectives

   To design a  mobile robot to move 3 different spheres into the ‘pen’ formed by two walls using teleoperator mode or autonomous mode.The robot needs to have a URDF file which defined to load into Gazebo in the simulation and be able to move and interact with objects in the simulation. 

## Design

  According to objective, design a robot with two fingeres can move the different sizes of spheres to the destination. 
  
    
 Model
  
  
  ![Capture model](https://user-images.githubusercontent.com/117764288/212550730-ead16d94-aafc-4113-aa00-a57f6f19e6f0.JPG)
  
  
  

To move different size of spheres, created robot with 3 wheel,Its a balanced robot having 2 guides/fingers to guide balls to pen/destination.In that one wheel is caster wheel, it will help robot for balance while moving.Also added body support to attach visual system.

## Packages

For our course work we added  packages like Assesement world,myrobot and pde4430_cw1.


  ![src](https://user-images.githubusercontent.com/117764288/212551390-add17eef-988c-4f7d-8e89-3dfb99b21bad.JPG)
  
## Simulation

   For simulation, in new terminal need to type "roslaunch myrobot myrobot.launch" , in this " myrobot" is package name and launch file is "myrobot.launch"
   
   ![myrobot launch](https://user-images.githubusercontent.com/117764288/212552600-e630df67-c0bb-457c-a16c-13458029aa48.JPG)
   
   in myrobot.launch file, called assessment_world, so world will create once myrobot.launch run.
   
   ![call](https://user-images.githubusercontent.com/117764288/212552919-9a4fefa7-4cb0-4de4-befe-3d39aab36d92.JPG)
   
   once run the terminal, RVIZ and Gazebo will open.In Gazebo, we can see robot with assessment world.
   
   ![assesssement world](https://user-images.githubusercontent.com/117764288/212553179-fd947cd8-3d4c-4c17-bb3b-efb0daab43c2.JPG)

   

   Then need to open new terminal  and type "roslaunch assessment_world objects.launch" for calling object in to the world.

   ![object launch](https://user-images.githubusercontent.com/117764288/212553015-75de1198-1967-45a6-b2b4-177c97528032.JPG)
   
   once run the terminal by enter key,  3 spheres will generate in the world.
   
   ![with objects](https://user-images.githubusercontent.com/117764288/212553282-0894d768-d42f-4cb4-baca-322c172c3a31.JPG)

   
   To move the spheres, using teleop method.For that ,open new terminal  and type "roslaunch myrobot rover_gazebo_teleop.launch" or type  " roslaunch pde4430_cw1 turtle_teleoperator.py"

![teleop launch](https://user-images.githubusercontent.com/117764288/212553698-ed1a29f2-fb02-4834-afc8-5a0de98a0e67.JPG)

 Press "enter"  key  and will run the program.And its shows which keys are used for the movement.
 
 ![teleop key](https://user-images.githubusercontent.com/117764288/212553989-09075d28-347d-40d4-999a-b3bda64e352b.JPG)

With help of teleoperation, can move the spheres in to the pen/destination point.While moving the robot, fingers/guide will help us to grab and guide  the spheres.

Accordingly we need to adjust the speed of linear / angular velocity while moving with balls.

![Captureggg](https://user-images.githubusercontent.com/117764288/212554126-8cd6e592-fb02-42c6-b643-b7efb5d30f52.JPG)

## Video

Youtubelink for video narration : 

## Reference

Following reference help me for this course work.

http://wiki.ros.org/urdf/Tutorials


## Conclusion

 This course help me to add knowledge about URDF,Gazebo, Rviz and how we can pluggin the python files with packages, run the world.It gives more idea to make robot with physical properties.




  
   

  

  
  







# Endless_runner
 
 ![gam](file:///C:/Users/Flux/Downloads/character%20move.png)
 
 ##### A

Project Report (Project-II) On

&quot; **Endless Runner&quot;**

**For the Degree of**

Bachelor of Engineering in Computer Science &amp; Engineering Submitted By,

**Mr. Pratik Kiran Patil Mr. Omkar Anil Patil Mr. Ganesh Ashok Patil**

**Mr. Chinmay Sanjay Hirave**

Under the Guidance of

**Prof. Sandeep G. Sutar**

![](RackMultipart20210401-4-1yv2m70_html_8610fe4a03ff3a4b.jpg)

Department of Computer Science &amp; Engineering

## Annasaheb Dange College of Engineering &amp; Technology, Ashta Tal. Walwa, Dist. Sangli, Maharashtra, India

&quot;_ **To be a Technological Institution of a Global Repute&quot;** _

## 2019-2020

Sant Dnyaneshwar Shikshan Sanstha&#39;s

**Annasaheb Dange College of Engineering and Technology, Ashta**

![](RackMultipart20210401-4-1yv2m70_html_d2c0eeb95fc1b38b.png)

**CERTIFICATE**

This is to certify that the project entitled **&quot;Endless Runner&#39;&#39;** , which is being partially submitted by,

**Mr. Pratik Kiran Patil Mr. Omkar Anil Patil Mr. Ganesh Ashok Patil**

**Mr. Chinmay Sanjay Hirave**

For the fulfillment of the course: **Project-I** of the **&#39;** Bachelor of Computer Science and Engineering&#39; of **Shivaji University, Kolhapur**. This is the bonafide work carried under my supervision and guidance during the year 2019-20.

Place: Ashta Date:

**Prof. Sandeep**** G. ****Sutar Dr. S. H.**** Bhandari**

Guide H.O.D

DepartmentofCSE Department ofCSE

**Director**

Annasaheb Dange College of Engineering &amp; Tech., Ashta

|
 | **INDEX** |
 |
| --- | --- | --- |
|

List of figures |
 | Page No.i |
| List of abbreviations |
 | ii |
|
1. **Introduction**
  1. Introduction
 |
 |
1 |
| 1.2 Necessity |
 | 2 |
| 1.3 Objectives |
 | 2 |
| 1.4 Theme |
 | 2 |
| 1.5 ReportOrganization |
 | 2 |
| **2. Literature Survey** |
 | 3 |
| **3. System Design** |
 | 4 |
| 3.1 Flow Chart |
 | 4 |
| 3.2 CharacterModule |
 | 5 |
| 3.3 MovementModule |
 | 5 |
| 3.4 Obstacle Module |
 | 5 |
| 3.5 CheckpointModule |
 | 5 |
| 3.6 PerformanceAnalysis |
 | 5 |
| **4. Experimental Setup and Results** |
 | 6 |
| 4.1 ToolsUsed |
 | 6 |
| 4.2 ExperimentalSetup |
 | 8 |
| 4.3 Result |
 | 9 |
| **5. Conclusion** |
 | 18 |
| 5.1 Conclusions |
 | 18 |
| 5.2 Applications |
 | 18 |
| **References** |
 | **I** |

**LIST OF FIGURES**

| **Fig. No.** | **Figure Name** | **Page No.** |
| --- | --- | --- |
| 1 | Flowchart | 4 |
| --- | --- | --- |
| 2 | Windows Application Output | 7 |
| 3 | Sample Obstacle | 8 |
| 4567891011 | Windows outputObstacle UsedCharacter MovementRamp UpRamp DownPick Up CoinsRight Corner TileSkeleton Mesh | 1011121314151617 |

i

**LIST OF ABBREVIATIONS**

| **Sr.**** No. **|** ACRONYM **|** FULL FORM** |
| --- | --- | --- |
| 1 | API | Application Program Interface |
| --- | --- | --- |
| 2 | AR | Augmented Reality |
| 3 | FPS | Frames Per Second |
| 4 | GUI | Graphical User Interface |
| 5 | MMORPGs | Massively multiplayer online role-playing game |
| 6 | OpenGL | Open Graphics Library |
| 7 | RPGs | Roll playing games |
| 8 | UnrealEd | Unreal Editor |
| 910
 | VRWYSIWYG
 | Virtual RealityWhat You See Is What You Get


 |

# **CHAPTER 1**

**Introduction**

Thischapterfocusesonintroductionofproposedsystem,objectivesoftheproposedsystem, theme and reportorganization.

1. **Introduction**
  1.
#### Introduction

The Unreal Engine [3], first released in the 1998 first-person shooter game, it is a game engine created by Epic Gaming. It has been successfully used in a number of other genres, including consoles, battle games, MMORPGs, and other RPGs, while initially developed for first-person shooters, the Unreal Engine features a high degree of portability with its code written in C++ and is a technology used today for many game developers, with source accessible. Unreal Engine4, which was launched in 2014, is the most recent version.

Collision detection, colored lighting, and a restricted method of texture filtering were among its applications. A level editor, UnrealEd, which had support for real-time positive solid geometry operations as early as 1996, was also built into the engine, enabling mappers to alter the level structure on the fly.

Endless Runner is an adventure game in the video game genre. The player-controlled character must jump and climb between given platforms in an endless runner, while avoiding obstacles. Environments also have rugged terrain that must be traversed at different elevations. To prevent causing their character to drop to their death or skip required hops, the player also has some control over the height and distance of jumps. The hop button remains the most popular unifying feature in games in this genre, but there are other alternatives now, such as swiping a joystick.

Initially, the system is depended on software processing, suggesting that the CPU was responsible for the graphics calculations. However, this was able to take advantage of the options offered by graphics cards, a method that allowed Sweeney to rewrite the core rendering algorithm 7 times. Also as practice, the founding program co-existed with software / hardware processing, with the latter concentrating on the Glide API, specifically developed for 3dfx accelerators. Though sponsored, due to the lack of texture management, OpenGL and Direct3D recorded slower performance relative to Glide.

  1.
#### Necessity

Need was felt to design and develop a game, due to growing anxiety and stress in society.

  1.
#### Objective

Objective 1: To create character and Obstacles.

Objective 2: To run the character on path.

Objective 3: To bypass obstacles controlled through keyboard keys.

Objective 4: Create checkpoints and add complexity level.

  1.
#### Theme

Themainthemeofourprojectis,itisaonekindofgame.Theapplicationprovidesanendless runnerenvironmentwhereinfiniterandomizedtilesaregeneratedwhereplayerhavetobypass obstacles to score points. The main advantage of this game is it helps to create brain activities, improves concentration power and increases hand to eyecoordination.

  1.
#### ReportOrganization

The project work involves the design, development and deployment of game. The study for the project is structured as follows:

    1.
###### Chapter 1:Introduction

Thissegmentfocusesonintroductionofproposedsystem,objectivesoftheproposedsystem, theme and reportorganization.

    1.
###### Chapter 2: LiteratureSurvey

Thissegment describesthevariouswebsiteswehadstudiedforunderstandingvariousconcepts and development of the projectwork.

    1.
###### Chapter 3: SystemDesign

The design of the basic project work structure, data flow diagrams, flow maps, sequence diagrams and class diagrams are described in this section.

    1.
###### Chapter 4: Experimental Setup andResults

This segment describes the experimental setup along with the details of the installation of softwarerequiredfordevelopmentoftheprojectandtheresultsachievedfromtheprojectwork.

    1.
###### Chapter 5:Conclusion

This segment describes the final conclusion obtained from the proposed system and also de- scribes the future work that can be done in the proposed system. It also describes the various applications of the project.

#### References

This chapter describes the various websites we studied for the understanding and thedevelopment of the projectwork.

# **CHAPTER**

#

# **2**

###

###

### Literature Survey

This chapter describes the various websites we had studied for understanding various concepts and development of the project work.

1.
### LiteratureSurvey

This YouTube channel [1] offers various courses showing how to make very own games from the ground up without any experience using game engines and apps. It offers videos for Unreal Engine 4, developing a First Person Shooter Game, Developing a Role Playing Game, Blender 3D Modeling Basics, and Game Creation Fundamentals.VideoofUnrealEngine 4GameDevelopmentFundamentalsisreferredforthisprojectdevelopment.

Unreal Engine 4 for developers is a full suite of real-time 3D software developed by developers. From PC, console, smartphone and VR gaming to cinematic simulations, visualizations and training tools, build and take the content everywhere. You get everything you need to launch, sail, rise and stand out from the audience with Unreal Engine [2].

Unreal engine 4 has been used for project production.

Details on the purchasing and distribution of the UE marketplace can be found in the official link to the UE [3].

The designed game characters are downloaded from the UE marketplace.

The tutorials on game development on everything from unreal engine to programming [4] assist in the design and development of the game.

# CHAPTER 3

### SystemDesign

The design of the basic project work architecture, data flow diagrams, flow maps, sequence diagrams and class diagrams are mentioned in this chapter.

1.
### SystemDesign

###

### This section describes the system design of the proposed system. System design is the process of designing the elements of a proposed system such as the architecture, flow diagram, different modules and methodologies and the data that goes through the system.

  1.
#### FlowChart

![](RackMultipart20210401-4-1yv2m70_html_e9bd46a0de6da709.jpg)

Figure1,describestheflowofproposedsystem. Gamebootingisaninitialpartofthisflowchart. After booting, current level is generated. This current level is an initial level where character spawns.Playerwillplaygamebypassingobstaclesandcollectingpoints. Whenplayerwillcollide withoneoftheobstaclesorifplayergoesoutofplayareathegamewillend.

When game ends by collision of obstacle and player it will generate a frame having two buttonsoneisrestartandanotherisleave. Thegamewillhaveapausebutton,ifplayerwantsto leave the game then player will press the leave button. If player press restart button the game willbestartedfrominitialpointandcharacterwillspawnagain.

If player press leave button the game will close. If player is not collided with obstacles then gamewillbecontinued.Thenewerandcomplexlevelsaregenerated.Thenewcomplexitylevels arerecognizedbycheckpoints.Checkpointsarethoseinstanceswheregamerecognizethat have to increase its complexity.

  1.
#### Module 1: CharacterModule

InthisproposedsystemmainpurposeistoCreateacharacter(playermodel)alsowearegoing toaddobstacles.Inthisproposedsystemthecharacterorplayermodelwhowillrunonthepath avoiding obstacles will be designed here as well as to develop a robot as a character, because humans can&#39;t runendlessly.

  1.
#### Module 2: MovementModule

Thismoduleproposesmovementsofcharacterbyusingkeyboardkeys.Inthisproposedsystem themovementsofplayerwillbecarriedouthere.Themovementslikejump,turnetc.areadded herebycodingusingthingslikeforwardvectoretc.alsospeedofcharacterinitiallyisgivenhere.

  1.
#### Module 3: ObstacleModule

This module proposes of adding obstacle avoidance through keyboard keys. The collision detection is one of the key point for this game. When a player strikes obstacle then game should terminate. If not then there is no importance for obstacles. Also if character goes out of bound/path then game should terminate too.

  1.
#### Module 4: CheckpointModule

Thismoduleproposesofaddingcheckpointswhichwillincreasecomplexitylevel.Morecomplex levels will be added in this module. When complexity (frequent obstacles, increase in speed) increases the brain activities will start acting as hand-eye coordination as well as increase in brainusage

  1.
#### Module 5: Performanceanalysis

In this module there will be testing of game and bug fixing. In this the environment and graphics will be rich. The GUI for player will also be great. The testing of this system will be alsodoneonunrealenginesinbuiltplatform.Sotheperformanceanalysistherearebenchmark like Fps(frames per second), in time criteria there is delay in ms. For having low delay there is need of high endcomputer.

# CHAPTER 4

### Experimental Setup and Results

This chapter describes the experimental setup along with the details of the installation of soft- ware required for development of the project and the results achieved from the project work.

1.
### Experimental Setup andResults

  1.
#### ToolsUsed

#### To develop this system it is necessary to use a framework that is Unreal engine version 4. This section describes the programming language and the different libraries which are used to develop this system.

1. **Unreal Engine**** 4**

Unreal Engine 4 is a full set of software for creation made for someone who deals with real-time technologies. Unreal Engine 4 gives you everything you need to start, ship, develop and stand out from the crowd, from business apps and cinematic experiences to high-quality gaming through PC, console, tablet, VR and AR.

A world-class tool set and open workflows allow developers to easily iterate concepts and see instant outcomes without touching a line of code, while complete source code access allows everybody in the Unreal Engine 4 ecosystem the ability to change and extend engine functionality. Its ruggedness is the greatest strength of an unreal engine. It is an advanced program that has a comfortable experience for consumers.

Unreal Engine is a real-time engine as well as editor with photorealistic rendering, dynamic physics and effects, realistic looking animation, reliable translation of information.

**Features of Unreal Engine 4:**

1. **Pipeline integration**

Easily automate data preparation workflows—even if you&#39;re not a programmer—with a simplified visual tool that lets you create a &quot;recipe&quot; of filters and operators that you can save and reuse on other scenes or projects. Make LODs, set up Light map UVs, substitute materials, and delete or merge objects based on factors such as class, name, metadata tags, or size.

1. **The Unreal Editor**

Unreal Engine includes the Unreal Editor, an integrated development environment available on Linux, MacOS, and Windows for content authoring. With support for multi-user editing, artists, designers, and developers can simultaneously make changes to the same Unreal Engine project in a safe and reliable way, while the ability to run the full Unreal Editor in VR mode means you can build in a WYSIWYG environment.

1. **Mesh editing tools**

Unreal Engine includes basic mesh editing tools to correct small problems in geometry without having to fix them in the source package and re-import. Within the Static Mesh Editor, you can select faces in a variety of ways—by picking, by material, by element, or with grow/shrink—and create, delete, or flip the selected faces, or detach them to a separate new static mesh. You can also unify normal, assign a new material, and perform basic UV projections

######

######

1.
###### Character animation tools

######

###### Completely customize characters and craft believable movement with Unreal Engine&#39;s mesh and animation editing tools, which include powerful features such as state machines, blend spaces, forward and inverse kinematics, physics-driven animation for ragdoll effects, and the ability to preview animation on the fly. A scriptable rigging system offers ways to achieve procedural rigging, animating in engine, or setting up custom retargeting or full-body IK solutions.

######

1.
###### Sophisticated lighting

######

###### Create realistic interior and exterior lighting effects while maintaining real-time performance, with a wide range of advanced lighting tools, including an atmospheric Sun and Sky environment, volumetric fog, volumetric light maps, precomputed lighting scenarios, and mesh distance fields.

######

######

1.
###### Virtual Texturing

######

###### Unreal Engine offers two methods to enable support for very large textures by dividing them into small tiles and only loading the visible tiles. Streaming Virtual Texturing, which uses Texel data from converted textures on disk, reduces texture memory overhead for light maps and detailed UDIM UV artist-created textures. Runtime Virtual Texturing, where Texel data is generated by the GPU at runtime, improves rendering performance for procedural and layered materials.

######

######

1.
###### Chaos physics and destruction system

######

######

###### Chaos is Unreal Engine&#39;s next-generation high-performance physics system. Using Chaos&#39;s Destruction feature, you can fracture, shatter, and demolish massive-scale scenes at cinematic quality with unprecedented levels of artistic control. Chaos also supports static mesh dynamics, cloth, hair, vehicles, and rigid-body animation, and is integrated with Niagara for secondary effects such as dust and smoke.

######

######

1.
###### Blueprint visual scripting system

######

###### With designer-friendly Blueprint visual scripting, you can rapidly prototype and ship interactive content without touching a line of code. Use Blueprints to build object behaviors and interactions, modify user interfaces, adjust input controls, and so much more. Visualize gameplay flow and inspect properties while testing your work using the powerful built-in debugger.

######

######

1.
###### Media Framework

######

###### The Media Framework enables the playback of videos inside Unreal Engine. Videos can be scrubbed, paused, or rewound inside a Media Player asset, as well as controlled through C++ or Blueprints Visual Scripting. Supported formats include a range of Apple ProRes formats on Windows, and video encoded with the HAP codec.

######

######

1.
###### Full access to C++ source code

######

###### With free access to the complete C++ source code, you can study, customize, extend, and debug the entire Unreal Engine, and complete your project without obstruction. Our source code repository on GitHub is continually updated as we develop features in our own mainline, so you don&#39;t even have to wait for the next product release to get your hands on the very latest code.

######

######

######

######

###### Unreal Engine Requirement

  1. Intel i3 Processor 4GBRAM

  1. Windows7/8/10

  1. Graphic card - Nvidia 940mxonward

  1. 1,024 x 768 or higher resolution display

  1. Keyboard &amp; Mouse

  1.
#### ExperimentalSetup

For this implementation we need to install Unreal engine with epic games installer.

###### Unreal engine installation steps

1. Go to unreal engine official website.
2. There is an installer available on website click on it.
3. Download and Run the Installer (Epic Games Launcher Set-Up Program)
4. Create an Epic Games Account (if you don&#39;t already have one)
5. Sign into the Epic Games Launcher.
6. Install the Unreal Engine4.
7. Install requiredplugins.
8. Launch the unreal engine.

**These are the following steps:**

1. **Go to unreal engine official website.**

For downloading go to website for download.

1. **There is an installer available on website click on it.**

Click on installer to download.

1. **Download and Run the Installer (Epic Games Launcher Set-Up Program)**

Downloadandinstallthe installer.

1. **Create an Epic Games Account (if you don&#39;t already have one)**

First create an epic games account.

1. **Sign into the Epic Games Launcher****.**

Sign in into epic games.

1. **Install the Unreal Engine**** 4.**

Install the unreal engine 4 latest software.

1. **Install required**** plugins.**

Install all the plugins that you required.

1. **Launch the unreal engine.**

Launch the unreal engine and you&#39;re ready to go.

  1.
#### Result

    1.
###### Windows applicationoutput

![](RackMultipart20210401-4-1yv2m70_html_c9deef56d4ced77f.jpg)

Figure 4.3.1: Windows Output

Figure4.3.1showsawindowsoutputforgame.ThegameisexportedinWindowsplatform. When it cook packages in unreal engine, the console log gives information about packaging process.

As shown in screenshot above there is a character running on path collecting coins, avoiding obstacles through keystrokes. We have built this game in an endless environment where player runs infinitely until he or she collides with obstacle that is rock or the player will collide on wall.

Collision is detected through unreal engines one of features that is collision detection. Collision detection is an inbuilt feature where it has all the functionality of detecting collisions.

Also as shown in the windows output screenshot above there in count of coins. It measures how many coins you have collected through out your one session. Coins that players collect are generated by coin generation code and its related function coin count. Here also we use collision detection method in which the player collides with our object coin and collision is detected and then our coin counter is increased by the collision count.

The collision detection is also used in situation like when player collides with wither wall or the obstacle we created that is rock. When player collides with the obstacle it will call player collide function in which the output is termination of current session. Similarly in case of wall collide the same player collide function will be called and current session will be exterminated. The collision detection occurs when one of the event called on component hit is started. This event will call necessary functions like death, coin generation and collision detection etc.

    1.
###### Obstacleused

![](RackMultipart20210401-4-1yv2m70_html_43dc470e372845c4.jpg)

Figure 4.3.2: Obstacle

Figure 4.3.2 shows sample obstacles in game. After colliding with obstacle character will die.

As shown in above screenshot the object highlighted with a yellow line is our obstacle &quot;rock&quot;. This obstacle is created with mesh structure and functionality. We can simulate this object in a specific environment if we want. As any other 3D object it also have three axes. We have transformed this object as one in all the three axes.

The static mesh of object is SM\_Rock, SM stands for static mesh. We can select other than this static meshes like wall, cone, and sphere as an obstacle. Also we can create our own static mesh object that is customized object or derived object. We can download any static meshes from unreal engine store as per project requirement.

The material used for this static mesh structure is M\_Rock. This material give the materiality to structure we provide. Basically static mesh is a skeleton and the material is skin to skeleton. Materials contain a large amount of textures and skins. Like static mesh you can buy the customized skins or textures from unreal engine 4 store.

As per game requirements we have added the collision detection to this object, so it could have original properties like rock. Disabling static mesh will hollow the rock object. In the construction script area there is ready to use library function.

As a 3D object our rock will have all the same functionality as a rigid rock in real life. We have added an explosion on colliding with rock, because our character is robot. In this system we have added a death function, when we attach any certain function with our death function or if we call death function then our session exterminates. Main factor here is an event which is called &quot;On component Hit&quot;, this event occurs whenever collision happens.

    1.
###### Charactermovement

![](RackMultipart20210401-4-1yv2m70_html_dfb9932818645fd7.png)

Figure 4.3.3: Character movement

Figure 4.3.3 shows movement of character. To change direction of character we use &quot;A&quot; and &quot;D&quot; keyboard keys.

The character movement module is one of the important module in which the character has given the ability to run in this endless environment. In this proposed system we have to run on endless path by avoiding obstacles. To avoid the obstacles we have given the character movement.

To move on the left side you have to press and hold the &quot;A&quot; key, to move to right you have to press and hold &quot;D&quot; key. We haven&#39;t made movement to stop as it breaks the concept of endless genre. Also the forward movement is fixed so no key pressing for forward movement.

For forward movement we have taken a vector which have a specific speed at which it runs, that is called forward vector. After some distance which is called checkpoints, the speed slightly increases to make the game interesting and adding difficulty to play.

We can&#39;t avoid obstacles by jumping over them from plane surfaces. But we can jump over them from a vertical distance, because our course or path is rigged. We have uncertain amount of up and down platforms. It is randomly generated through our random generator function.

For jumping of character we have given an upward vector. We have given this vector an upward force 5f at Y-axis. For jumping we have assigned space key. After some time the gravity acts on our character and character starts to fall down. You cannot jump in air twice, because there is no rigid surface to jump on. Also jumping simultaneously slightly increases speed. If character dies by going outside bound or path the character dies and terminates current session. Character dies when it goes below X-axis (below 0.0).

    1.
###### Ramp up

![](RackMultipart20210401-4-1yv2m70_html_f0953d6a20cfdf7a.jpg)

Figure 4.3.4: Ramp up

Figure 4.3.4 show the track on which character will run. Obstacles and coins will be present on this ramp.

As mentioned above this is path on which character will run. This path consists of small parts called tiles. This tiles are only designed once, after that we put them in loop where they are generated infinitely. That is what we call infinite random tile generation. First we take 10 similar straight path where character can run and we can apply our loop.

We use a function named random integer in range to get a randomized output. We take that random input and place it at last index of tenth tile as it can generate forward. As shown in above figure there are some spawn coins and blocker. They are also randomized using random integer in range. For coin spawning on path we have used for loop up to 5 iterations.

In above figure there is bounding entity which helps us to generate within a specific area. The bounding entity is a hollow cube which allocates specific component within its range. We can take example of coin we have declared an area named coin area where we generate or spawn our coins.

The next upcoming tiles are connected with spawn points, they are red arrows as shown in above figure. We connect path tiles, upward and downward slopes to our spawn points. We take those relative point and store them in array to set points. When we simulate our path we can see our coins and blocker generating randomly.

There are two walls attached on both of its sides, those walls are also used to for our corner tile. Where if we don&#39;t rotate our character in 90 degrees, then it will face wall head on and die with explosion. Here for generating continuous tiles one after another we have used end Trigger function, it is a trigger box which triggers specific events after coming in contact with them. You can see end trigger box vertical at slope or upward ramp.

    1. **Ramp down**

![](RackMultipart20210401-4-1yv2m70_html_9d3d27f0e0a38fd4.png)

Figure 4.3.5: Ramp down

Figure 4.3.5 show the track downwards for ramp. Coins and obstacles will be present on this ramp

As above mentioned, figure shows a ramp down tile. This ramp down tile has an end trigger box, which follows certain pattern to generate randomized tiles. The trigger box depends on condition you provide to its function. The red arrows are spawn points which helps to generate trigger boxes and next iteration of randomized tiles. When we simulate this tile we get some random blockers &amp; coins.

It is surrounded two walls for bounding the path to certainty. Spawn points are used to spawn the slopes and upward ridges. Those slopes and ridges are also static meshes that is they are structure. They also have real life properties, we have given them sand and soil material for looking like real slopes of sand. We can also give rocky ridges or slippery slopes. We just have to select another static meshes and material from given options. The static mesh used is a shape\_wedge\_B and material is M\_concrete\_grime.

Also we have used cube static mesh for surface or tile &amp; the material use for surface is M\_ground\_grass. The dimension for surface tile is 10 on X-axis, 10 on Y-axis and 0.1 on Z-axis. The two side walls are cube static meshes with dimensions of 10 on X-axis, 0.1 on Y-axis and 0.2 on Z-axis &amp; the material used for wall is M\_brick\_clay\_new which gives brick like skin to wall. Wall are placed at +500 &amp; -500 on X-axis also they +100 on Y-axis (height).

Side walls are not designed to destruct our character. Only face on walls are destructive as per endless runner genre rules. Shadows and lighting are default by system and are also as per environments. Because by turning on path it can have a situation where there is less light from sun that is sky light, therefore less vision in game.

    1.
###### Pick upCoins

###### ![](RackMultipart20210401-4-1yv2m70_html_d3fc70ea6612c015.jpg)

######

Figure 4.3.6: Pick up Coins

Figure4.3.6showthecoinwhichcharacterwillcollectwhileplayingthegame.Itwillappear randomly on theramp.

As mentioned in above figure description it is a coin which is made up of static mesh. The static mesh we used for this coin is shape\_torus. To make it look like a real coin we have given the material that is M\_metal\_gold. Basically torus is horizontal shaped so we have to rotate it 90 degrees. These coins are generated randomly in a coin area. There are 6 coins which are randomly generated in a bounding box. As you can see the torus shape is a 3D shape having three axes. Below torus that is our coin we have given a point light which gives glowing effect. The point lights comes under directional lighting type where light is spread on certain directions. Directional lights includes other lights like spot light rect light &amp; sky light.

We have used sky light to our project as a provider of light most of time. In simple words sky light acts as a sun in real time entity, sky light spreads in multi directions. Spot light is used to illuminate a specific area in dark. In real world bulb is example of spot light. The point light shows light in single direction, the real time example of point light would be torch.

To make our coin more visible and entertaining to watch we have added some circular momentum to it. It rotates 360 degrees clockwise. Also we have added coin pick up sound to it as it someone picking up stash of coins. The coins are collected and added to score board by a function used that is on component overlap. This function is casted to our running character, when our character overlaps a coin, the add coin function will be called and coin will be disappeared &amp; added on score board. When character overlaps a coin the sound will be generated at the exact time.

After overlapping a coin will be destroyed by using destroy self or destroy actor function. We destroy coin to avoid visible confusion. Our overlap function comes under collision detection, as player collides with a coin. We have generated an overlap event which will simulate to see that character is picking up coins. There are generally three condition on overlap functions first in &quot;OnActorBeginOverlap&quot; this condition executes when we first came in contact with any physical entity, in our case its coin. Second condition is &quot;OnActorEndOverlap&quot; this executes at the exact moment when actor that is character had passed through physical entity that is coin. And last condition is &quot;OnActorHit&quot; where after passing through entity (coin). This function will destroy our entity to avoid unnecessary visible confusion.

    1. **Right corner tile**

![](RackMultipart20210401-4-1yv2m70_html_2b987ddb35d6e17e.jpg)

Figure 4.3.7: Right Corner tile

Figure 4.3.5 shows the corner tile. From this tile, character will turn in 90 degree right.

As above mentioned this is a right cornered tile. This is where character takes turn and changes as path changes. As you can see there is a big cubical box outline, which is also called as Turn zone. Basically Turn zone is used to divert character in a certain directions by giving specific inputs. The turn zone have two types first is by turning left or by turning right. When you hit a corner wall head on the character will be destroyed as per endless runner rules. To turn right player has to press &quot;D&quot; key &amp; to turn left press &quot;A&quot; key.

The red arrows are called spawn points, they decide where to generate a tile next. There is box outlined entity above the spawn point which is called an end trigger box. Which is used to generate random tiles next to it. So a corner tile basically consists three areas first is coin area where coins and blockers are generated randomly. Second is End Trigger box and third is turn zone. The working of turn zone is as similar as coin pick up, as they use same kind of functions.

When players enters into a turn zone he have to give input to turn if he wants to survive. The function used for this is On Component Begin Overlap. This function is casted to our character, then we set its value to variable where we enable the option can turn. Can turn is a Boolean type variable where there are only two conditions true or false. We attached our can turn variables to our &quot;A&quot; and &quot;D&quot; key, after that we set up a desired rotation whereas its variable type is a rotator. By getting and setting out desired turns and appointing to key the character turns. The axes we used for turning is Z axis we rotate at -90 to rotate left and +90 to rotate right. To turn corner we created a custom event at top.

    1. Skeleton mesh

![](RackMultipart20210401-4-1yv2m70_html_6a6f6f5d8fff3611.png)

Figure 4.3.8: Skeleton Mesh

Figure 4.3.8 shows skeleton mesh of running character. Behind skeleton camera is fixed.

The skeleton mesh is mesh variable of character category. The capsule around skeleton is used to encapsulate the character entity. The camera behind acts as POV (point of view). The player who&#39;s playing will see this point of view. We can change POV as per requirements. There are major two types of POV first is TPP (Third Person Perspective) &amp; second is FPP (First Person Perspective). Currently we are using TPP as per endless genre rules. FPP is mostly used in FPS (First person shooter) games.

We can change the static mesh and material used for our character. The current static mesh used for this component is SK\_Mannequin &amp; the material used for this skeleton are M\_UE4Man\_Body and M\_UE4Man\_ChestLogo. As this is a human entity in game we have enabled gravity, shadowing &amp; collision rules. The default animation class is used in this project as we are not developing an open world environment. The default animation class includes all directional movements like human body.

The functions which are used in character movement are mainly attached and used in this character mesh script. For continuous moving of a character we have used a forward vector. To rotate or turn our character we take a get rotation vector and give its output to make rotator function. The one of the important script is death and it&#39;s declared in character construction script &amp; it is used by other classes by inheriting this script class. We create a custom event for death of our character, for this we have used a spawn emitter which gets the character location and destroys the character. Then the output of emitter is forwarded to location sounds which gives explosion sound. After the death of character there is delay of 2 sec to restart the game. The get actor location function return its values that is location to spawn emitter and location sound.

# CHAPTER 5

### Conclusion

Thischapterdescribesthefinalconclusionobtainedfromtheproposedsystemandalsodescribes the future work that can be done in the proposed system. It also describes the various application of theproject.

1.
### Conclusion

  1.
#### Conclusions

In this project we have developed a basic 3D game. In this game, we have designed a character, which runs in the direction set by W-A-S-D keys on keyboard.

  1.
#### Applications

Endless runner game is designed for people from any age group. This game may be used for entertainment or for stress relief purpose.

# References

1. Charactermodelforgame[online]Availableat:h[ttps://www.mixamo.com](http://www.mixamo.com/) Last accessed :10/09/2019

1. Tutorials for game development [online] Available at : h[ttps://www.y](http://www.youtube.com/user/VirtusEdu)outub[e.com/user/VirtusEdu](http://www.youtube.com/user/VirtusEdu)Last accessed :30/07/2019

1. Enginedownloadsite[online]Availableat:h[ttps://www.unrealengine.com/marketplace/en-](http://www.unrealengine.com/marketplace/en-)US/free

Last accessed: 30/07/2019

1. Assets for game [online] Available at :h[ttps://ww](http://www.devassets.com/)w.dev[assets.com](http://www.devassets.com/)Last accessed :03/09/2019

1. Tutorialsforenvironmentdevelopment[online]Availableat:h[ttps://www.y](http://www.youtube.com/user/UnrealDevelo)outub[e.com/user/UnrealDevelo](http://www.youtube.com/user/UnrealDevelo)Last accessed :23/08/2019

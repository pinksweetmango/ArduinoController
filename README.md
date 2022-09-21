  
Use other features of an Adafruit Circuit Playground as an input device in a Processing program
===============================================================================================
![](CircuitPlaygroundLabeled.jpg)    
In this Arduino lab you will write a program that uses other features of the Adafruit Circuit Playground as an controller for a Processing program. The circuit playground has 16 inputs. Adafruit has a detailed description [here](https://learn.adafruit.com/introducing-circuit-playground/guided-tour). In addition to the light sensor that we used in the previous assignment, the circuit playground also has a:
* Temperature Sensor
* Microphone Audio Sensor
* Motion Sensor
* A 3-axis accelerometer
* Capacitive Touch sensor
* Two large left and right buttons
* Slide switch 

Here's a sample program that will print the values of 16 inputs. Run the program and then press, touch and manipulate the various sensors to see how they work.
```java {.line-numbers}
import processing.serial.*;
import cc.arduino.*;
Arduino arduino;

public void setup() {
  size(100, 100);
  arduino = new Arduino(this, Arduino.list()[0], 57600); //change the [0] to a [1] or [2] etc. if your program doesn't work
}

public void draw() {
  background(192);
  for(int i = 0; i < 16; i++)
    System.out.print(i+" "+arduino.analogRead(i) + "\t");
  System.out.println();
}
```
Write your own program
----------------------
Using the sample program as a guide, write your own program that uses one or more of the inputs. You may find slides 117 - 120 of the [apjavaProcessing slide presentation](https://docs.google.com/presentation/d/1sqbareaFmF9fMcp0XOl3hRO6hAlrU5WIaj4V-Kd3eDI/edit?usp=sharing) helpful. Your program doesn't have to work or look like any other, you can add more features to your previous virtual pet program or create a new one. Have fun and be creative! 

When you are happy with your program, have a friend make a short video of you using your program. The video need only show your hand, the arduino and your program's output, please don't include anyone's face in the video. Convert the video to an animated gif using a free converter like [ezgif.com](https://ezgif.com/). Use ezgif's *cut video* or a similar option to edit your video to under 10 seconds and less than 25MB. Upload your animated gif to your VirtualPet repository. Submit the link to your gif to Google Classroom. Don't forget to click the *Mark as done* button. 

Samples of Student Work
-----------------------
[Zoey](https://github.com/zoeyzhu/VirtualPet/blob/gh-pages/IMG_8459.GIF)  
[Jocelyn](https://github.com/jxcelynyu/VirtualPet/blob/gh-pages/IMG_0596.GIF)   
[Viva](https://github.com/vivavoong/VirtualPet/blob/gh-pages/processing_differentinputs.gif)   
[Kaitlin](https://github.com/kaiyenpepper/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20(2).gif)   
[Tiffany](https://github.com/tiffanyt11/VirtualPet/blob/gh-pages/845f586ee71d4459bf3b82f9efcedebb.gif)   
[Michelle](https://github.com/mitan4/VirtualPet/blob/gh-pages/bird.gif)   
[Jimmy](https://github.com/Jimmy1433223/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Alex](https://github.com/AlexHackathon/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20(1).gif)   
[Cameron](https://github.com/CaNguyen1/VirtualPet/blob/gh-pages/IMG_6116.GIF)   
[Mikey](https://github.com/miosullivan/ArduinoController/blob/main/ezgif.com-gif-maker%20(1).gif)   
[Nash](https://github.com/MoonNash/VirtualPet/blob/gh-pages/IMG_2876.GIF)   
[Federico](https://github.com/feaprile/ArduinoController/blob/main/ezgif.com-gif-maker%20(1).gif)   
[Koey](https://github.com/koeychan/VirtualPet/blob/gh-pages/ezgif.com-video-to-gif.gif)   
[Kenny](https://github.com/KennyCh13/VirtualPet/blob/gh-pages/Use%20other%20inputs%20of%20an%20Adafruit%20Circuit%20Playground%20in%20a%20Processing%20program.gif)   
[Leah](https://github.com/Lloyd2202/ArduinoController/blob/main/ezgif.com-gif-maker%20(1).gif)   
[Albert](https://github.com/alshi31/VirtualPet/blob/gh-pages/Albert%20Shi's%20Adafruit%20Circuit%20Playground%20GIF.gif)   
[Tiffany](https://github.com/TILOUIE2/VirtualPet/blob/gh-pages/season_gif.gif)   
[Keneth](https://github.com/KenethL/VirtualPet/blob/gh-pages/Arduino%20Game.gif)   
[Pansy](https://github.com/pakuang/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20(1).gif)   
[Johnny](https://github.com/Jlin202/VirtualPet/blob/gh-pages/ezgif-4%20final-b2ff005a7942.gif)   
[Chris](https://github.com/TophTheBro/ArduinoController/blob/main/ezgif.com-gif-maker.gif)   
[Sam](https://github.com/SamRosenblum415/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20(1).gif)   
[Tyler](https://github.com/ty237/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20(3).gif)   
[Karina](https://github.com/kaanders17/ArduinoController/blob/main/Arduino%20Controller%20GIF.GIF)   
[Bruno](https://github.com/bruno-415/VirtualPet/blob/gh-pages/ufo)   
[Damian](https://github.com/dabogdon/ArduinoController/blob/main/ezgif-4-0ce17385d59a.gif)   
[Paolo](https://github.com/paolo415/VirtualPet/blob/gh-pages/lightSensorShark.gif)   
[William](https://github.com/wicao1/VirtualPet/blob/gh-pages/other_arduino_buttons.gif)   
[Alvin](https://github.com/alchan6/VirtualPet/blob/gh-pages/Other%20Arduino%20Sensor.gif)   
[Christina](https://github.com/christina88chan/VirtualPet/blob/0c54b695443327fda79e071b026affb0292311e8/ezgif.com-gif-maker.gif)    
[Haden](https://github.com/hachan-beep/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%282%29.gif)   
[Joanne](https://github.com/joannechenn/ArduinoController/blob/main/ezgif.com-gif-maker%20%281%29.gif)   
[Irisa](https://github.com/irisac415/ArduinoController/blob/main/Fish%20Buttons.gif)   
[Christopher](https://github.com/ChGee/VirtualPet/blob/gh-pages/135C22BA-F855-477C-B751-C6C8E86F66B6.gif)   
[Wing](https://github.com/wilai3/ArduinoController/blob/main/ezgif.com-gif-maker%20%282%29.gif)   
[Caitlyn](https://github.com/calam1818/VirtualPet/blob/gh-pages/ezgif-2-ad9d63fa07a1.gif)   
[Breanna](https://github.com/brlau6/VirtualPet/blob/gh-pages/Abstract%20Rainbow%20Lines%20-%20Buttons%20and%20Light%20Sensor.gif)   
[Matthew](https://github.com/malee8/VirtualPet/blob/gh-pages/IMG_3427.GIF)   
[Ye](https://github.com/YejinL12/VirtualPet/blob/417992b7f3a6ce451937e2eb7658ad4ae9a4c743/colorfulOcto.gif)   
[Van](https://github.com/Vanthebot/VirtualPet/blob/gh-pages/otherArduinoSensor.gif)   
[Joshua](https://github.com/jopaza21/OtherArduinoSensors)   
[Edward](https://github.com/edpilotte/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Aiden](https://github.com/AidenShiu/VirtualPet/blob/gh-pages/ezgif-7-f278d7c40663.gif)   
[Andrew](https://github.com/antan2/VirtualPet/blob/gh-pages/buttons%20gif.gif)   
[Jeffrey](https://github.com/jethiDaCoder/VirtualPet/blob/gh-pages/Ping%20Pong.GIF)   
[Eric](https://github.com/desolaterakan/VirtualPet/blob/gh-pages/froog.gif)   
[Dylan](https://github.com/dy-alt/VirtualPet/blob/gh-pages/otherButtonsGif.gif)   
[Mira](https://github.com/mira16-v/VirtualPet/blob/gh-pages/other_sensor_GIF.gif)   
[Austin](https://drive.google.com/file/d/1D1Qi2s2Je5oXO8p3k0hUTvZQGbxz4wwr/view)   
[Jason](https://github.com/jawong32/Flappy)   
[Ivana](https://github.com/ivxu24/VirtualPet/blob/gh-pages/ezgif.com-video-to-gif.gif)   
[Gary](https://github.com/Gary055/anime/blob/main/ezgif.com-gif-maker%20%281%29.gif)   
[Emily](https://github.com/emyip/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Akemi](https://github.com/Akemi1222/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[William](https://github.com/WilliamsGitHubAccount/VirtualPet/blob/gh-pages/button_test.gif)   
[Stephen](https://github.com/stevenmeap/VirtualPet/blob/gh-pages/SnowManButton.gif)   
[Daniel](https://github.com/wood09/VirtualPet/blob/gh-pages/other_arduino_sensor-gif.gif)   
[Andrew](https://github.com/guppies23456/VirtualPet/blob/gh-pages/Other%20Sensor.gif)   
[Luke](https://github.com/LukeD808/VirtualPet/blob/gh-pages/LukeDonohueVirtualPetGif.gif)   
[Liam](https://github.com/ligiraldo/ArduinoController/blob/main/ezgif.com-gif-maker%20%281%29.gif)   
[Hayden](https://github.com/hakwok/VirtualPet/blob/gh-pages/gif-min.gif)   
[Jacob](https://github.com/jalambert/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Noella](https://github.com/noellalee1/VirtualPet/blob/gh-pages/D67067A3-0B42-4B34-8E5A-B5D9C5BB22CC.gif)   
[Caleb](https://github.com/caleung3/Snowman/blob/gh-pages/ezgif.com-gif-maker%20%284%29.gif)   
[Gabriel](https://github.com/galeung24/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Eric](https://github.com/ErLiao137/VirtualPet/blob/gh-pages/extra.arduino_gif.gif)   
[Joyce](https://drive.google.com/file/d/1B0qGeG1GO1Ip8Lg396Iwsc7S9PzcdVUQ/view)   
[Vivian](https://github.com/VivianMak/VirtualPet/blob/gh-pages/Other%20Arduino%20Sensors.gif)   
[Lexian](https://github.com/lexiannguyen/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Raina](https://drive.google.com/file/d/1xyOufV5JOFBs4oal3BEyj9Wa2SkbgPRc/view)   
[Rafael](https://github.com/IamRafaelllll/VirtualPet/blob/gh-pages/ezgif-3-8945803d9402.gif)   
[Nathaniel](https://github.com/NathanTjong/VirtualPet/blob/gh-pages/D29BD7F0-F638-4114-BDD5-F430A6F304E6.gif)   
[Nicolas](https://github.com/nireiss/VirtualPet/blob/gh-pages/sensorArduino.gif)   
[Brian](https://github.com/brsen/VirtualPet/blob/gh-pages/arduinoGameGIF.gif)   
[Justin](https://github.com/jushiu/Animation-2.0/blob/main/39F16F3D-26FB-45C0-B100-81D9FDC9A58F.gif)   
[Stella](https://github.com/StellaSit0/VirtualPet/blob/gh-pages/20210907_090630_1.gif)   
[Wendy](https://github.com/lafmj/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Joseph](https://github.com/JosephTeng/VirtualPet/blob/gh-pages/D0B5074F-26BA-4D05-BA87-E21E80FAE2A9.gif)   
[Joshua](https://github.com/jovegher/VirtualPet/blob/gh-pages/virtualcattemp.gif)   
[Brianna](https://github.com/brwong8/VirtualPet/blob/gh-pages/ezgif.com-video-to-gif%203.gif)   
[Justin](https://github.com/Justin-pyth/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Qiaoyan](https://github.com/QIAOYANX/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%282%29.gif)   
[Antonio](https://drive.google.com/file/d/11ZHX5IiykP8i5Yy4sSdWhpnMpqXj5duz/view)   
[Caden](https://github.com/cayeung1/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[TommyJun](https://github.com/toyu3/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[David](https://github.com/davidzhang3/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Darren](https://github.com/DarrenZhao1/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%202.gif)   
[Emily](https://github.com/huishancai/VirtualPet/blob/gh-pages/ezgif.com-video-to-gif%203.gif)   
[Brennan](https://github.com/Brennan-c/VirtualPet/blob/gh-pages/otherSensor.gif)   
[Jennifer](https://github.com/jennifer0525/VirtualPet/blob/gh-pages/Other%20Senors%20Virtual%20Pet.gif)   
[Deion](https://github.com/deionchaudhary/Panda/blob/gh-pages/otherArduinoSensors.gif)   
[Aaron](https://github.com/AaronnChen/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Jackie](https://github.com/jachen16/VirtualPet/blob/gh-pages/Other-Arduino-Sensors-Sep-3-2021.gif)   
[Christina](https://github.com/chchung1/VirtualPet/blob/gh-pages/other%20sensors.gif)   
[Joselino](https://github.com/joselinodt/VirtualPet/blob/gh-pages/IMG-9486.GIF)   
[Nathan](https://github.com/Naguan1/VirtualPet/blob/1741ad2cc41ccf1f048c3201c56ea2ba20c8e3ae/ezgif.com-gif-maker%20%283%29.gif)   
[Munkhtushie](https://github.com/tushigitgel/VirtualPet/blob/gh-pages/ezgifotherarduino.gif)   
[Kyle](https://github.com/kylam1/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Noelle](https://github.com/noellelam/VirtualPet/blob/441fd125be9c1d5632d927bda3cb7f072426e491/ezgif.com-gif-maker.gif)   
[Andy](https://github.com/andeey3/VirtualPet/blob/gh-pages/ezgif-4-5a1c7e858863.gif)   
[Audrey](https://github.com/AudreyLau8/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[William](https://github.com/Williamlaw2005/VirtualPet/blob/gh-pages/other%20sensor%20gif.gif)   
[Jenna](https://github.com/Jenna1910/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Ryan](https://github.com/chknwngs999/VirtualPet/blob/gh-pages/arduinoinput.gif)   
[Nathan](https://github.com/naleung1/VirtualPet/blob/gh-pages/Pet%20Slime%20Other%20Sensors%20gif.gif)   
[Ivy](https://github.com/ivyylin/VirtualPet/blob/gh-pages/F91185D6-8317-42C5-912E-9E40B56CEBE4.gif)   
[Gabriel](https://github.com/Gabriel-Low-06/VirtualPet/blob/cca8b9214e7182c2f70d30e52469fd062d8636ec/Flappy_With_Arduino.gif)   
[Joyce](https://github.com/joycema212/VirtualPet/blob/gh-pages/ezgif.com-video-to-gif%202.gif)   
[Pyry](https://github.com/Pyrym24/VirtualPet/blob/gh-pages/ButtonGif.gif)   
[Mika](https://github.com/mikanguyenn/VirtualPet/blob/gh-pages/OtherArduinoSensors.gif)   
[Sophia](https://github.com/sophiapeckner/VirtualPet/blob/gh-pages/FlappyCardinalOtherSensor.gif)   
[Ethan](https://github.com/Etqiu/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%282%29.gif)   
[Emely](https://github.com/emsarcenobravo/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%282%29.gif)   
[Nate](https://github.com/Nsirival/VirtualPet/blob/gh-pages/Nate%20Sirivallop%20-%20other%20sensors.gif)   
[Koen](https://drive.google.com/file/d/1vekV2_REgA5VCXll-2N1N42baFDVVmXa/view)   
[Annie](https://github.com/anxu9/VirtualPet/blob/gh-pages/cookie.gif)   
[Brayden](https://github.com/B-r-4-y-d-3-n/VirtualPet/blob/gh-pages/ezgif-4-996eba0ef3d6.gif)   
[Jason](https://github.com/JasonZhong3/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%283%29.gif)   
[Ivan](https://github.com/ivzhu1/VirtualPet/blob/gh-pages/ColorChange.gif)   
[Tobias](https://github.com/TobyZuercher/VirtualPet/blob/gh-pages/image0.gif)   
[James](https://github.com/JamesBackstrom43/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20(1).gif)   
[Kathleen](https://github.com/kathb3/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20(1).gif)    
[Juan](https://github.com/jucalvohuerta/VirtualPet/blob/gh-pages/OtherSensorsProjectJuan.GIF)   
[Toby](https://github.com/tobyjchan/VirtualPet/blob/gh-pages/IMG_0482.GIF)    
[Ryan](https://github.com/rchen0902/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Ryan](https://github.com/rychick/VirtualPet/blob/gh-pages/Ryan%20Chick%20-%20Other%20Arduino%20Sensors.gif)    
[Evangeline](https://github.com/evchien/VirtualPet/blob/gh-pages/otherSensor.gif)   
[Miriam](https://github.com/mifreedman/VirtualPet/blob/26a7cf350f0e7b239873778273ca695186d804c7/otherSensorGIF.gif)   
[Loren](https://github.com/l0renGigi123/ArduinoController/blob/main/ezgif.com-gif-maker%20%281%29.gif)    
[Sally](https://github.com/sahong3/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)    
[Tennyson](https://github.com/Tehuang1/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Allynaraizel](https://github.com/allynaj/VirtualPet/blob/27ed6f057a425ccbb128d755443ebe742931a6bf/F3668C50-5B84-44E1-89ED-9BB745DE288B.gif)     
[Alvin](https://github.com/allau1/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Sonia](https://github.com/sonia-who/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)    
[AndreiRock](https://github.com/Anliterato/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)    
[Maxwell](https://github.com/MaxAPCS/VirtualPet/blob/arduino/other_sensors.gif)   
[Humphrey](https://github.com/humphreyylu/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)  
[Hannah](https://github.com/hannahlucas987/VirtualPet/blob/gh-pages/ezgif-5-ed8bc01250.gif) 
[Fiona](https://github.com/f-iona/VirtualPet/blob/gh-pages/other_sensor_piggggg.gif)    
[Isaac](https://github.com/isaacmai/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Karla](https://github.com/karla0311/Virtual-Pet/blob/gh-pages/OtherArduinoSensors.gif)   
[Saw](https://github.com/SawYN01/VirtualPet/blob/gh-pages/other%20arduino%20controllers.gif)    
[Aiden](https://github.com/AiP24/VirtualPet/blob/gh-pages/assets/sukon-accel.gif)   
[Theo](https://github.com/JSSuperior/VirtualPet/blob/gh-pages/IMG_4375.gif)   
[Tara](https://github.com/Tara-Tiong/VirtualPet/blob/gh-pages/starslightup.gif)   
[Maya](https://github.com/mawang4/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Dylan](https://github.com/dylanwei1/VirtualPet/blob/aafec85ba7a98b1d84944f89ef3d001102742a8f/other%20sensors.gif)    
[Nicholas](https://github.com/Quantalope/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)    
[Samson](https://github.com/xusamson8/VirtualPet/blob/95433a0d51e344544eaa5ec377a0353618a1809e/button_pig_gif.gif)    
[Patrick](https://github.com/PatYAO/VirtualPet/blob/gh-pages/5610AA89-3780-4432-8465-ACCDDFB821AB.gif)    
[Diego](https://github.com/DiegoYuHuang/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Luca](https://github.com/luca321222/VirtualPet/blob/f2b8f8442a27055864518099709ce9b81e13a804/2C177777-BCA7-4F70-8682-CFAE9AE72022.gif)   
[Cuiyin](https://github.com/anna-c2/VirtualPet/blob/gh-pages/BBBF9CD5-277F-4A9F-949A-3D741F978700.gif)    
[Laura](https://github.com/lachen2/VirtualPet/blob/gh-pages/VirtualPet%20%282%29.GIF)   
[Noel](https://github.com/NOCHEN1/VirtualPet/blob/88b4a8fa0b7aa374ccfde4fb027ee8a2ccb3c482/ezgif.com-gif-maker%208.gif)   
[YiYuan](https://github.com/2005benchen/VirtualPet/blob/gh-pages/20220907_120838.gif)   
[Artiom](https://github.com/lilrussian/VirtualPet/blob/gh-pages/ezgif-3-3c346750bc.gif)   
[Marina](https://github.com/mderisi/VirtualPet/blob/gh-pages/MDeRisiArduinoSensors.gif)   
[Kevin](https://github.com/smallkedo/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%282%29.gif)    
[Samantha](https://github.com/sagee1/VirtualPet/blob/gh-pages/ezgif-5-a728ad1d4b.gif)   
[Charlotte](https://github.com/ssrendiptiy/VirtualPetTurtle/blob/gh-pages/83F3EAA1-DD61-4256-A5F7-60E7603B7AC1.gif)   
[Dylan](https://github.com/dylanh8/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%283%29.gif)    
[Joanna](https://github.com/2sekai/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%2828%29.gif)   
[Andy](https://github.com/kxnzite/VirtualPet/blob/gh-pages/other%20arduino%20sensors.gif)   
[Victor](https://github.com/Vi-L/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)    
[Ivan](https://github.com/ivli1/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Kaijun](https://github.com/KawaiiKai/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Michelle](https://github.com/michelle4570/ArduinoController/blob/main/ezgif-2-4f14a34606.gif)    
[Kyle](https://github.com/kyle-v420/ArduinoController/blob/main/ezgif-2-d0df332162.gif)   
[Jerry](https://github.com/J3RRRRY/VirtualPet/blob/gh-pages/Black_to_White__White_to_Black_MOV_AdobeExpress.gif)    
[Gage](https://github.com/gschopen/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)    
[Angela](https://github.com/angieela/VirtualPet/blob/gh-pages/FF0AAA73-F33B-49F5-A945-870293E7E676.gif)   
[Diego](https://github.com/diegooroyale/ArduinoController/blob/main/IMG_3466.GIF)   
[Ivona](https://github.com/ivonasutilovic1/VirtualPet/blob/gh-pages/unnamed.gif)    
[Sandy](https://github.com/satam2/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Johnathan](https://github.com/jotran6/VirtualPet/blob/gh-pages/ezgif-4-e2dba5d28b.gif)   
[KaloonRidge](https://github.com/ridgeWalkerSchool/VirtualPet/blob/26f799e42500a819147d7f531e4d42a271d83f5a/ezgif.com-gif-maker.gif)    
[Robin](https://github.com/Robin-Win/ArduinoController/blob/main/ezgif.com-gif-maker%20%281%29.gif)   
[Kayla](https://github.com/kawong2/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%282%29.gif)    
[Justin](https://github.com/Daqk1/VirtualPet/blob/gh-pages/image0%20%281%29.gif)    
[Leanna](https://github.com/lewu7/MyVirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Philix](https://github.com/philix/VirtualPet/blob/gh-pages/D4670947-24E8-4082-AC04-40E435C7AED6.gif)   
[Lixin](https://github.com/Oliveragel/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Audrey](https://github.com/audreyyann/VirtualPet/blob/b8eabcac08095b57ec44feabe4d05b716cd42b09/ezgif.com-gif-maker%20%282%29.gif)    
[Emily](https://github.com/emyang1/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)    
[Haoheng](https://github.com/HaoxD123/VirtualPet/blob/gh-pages/Another%20Ardurino.gif)    
[Gabriel](https://github.com/GabrielZub/VirtualPet/blob/gh-pages/ezgif-2-a57f684329.gif)    
[Alejandro](https://github.com/Alejandrofpv/ArduinoController/blob/main/ezgif.com-gif-maker%20%282%29.gif)    
[Angela](https://github.com/angelachen690/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%282%29.gif)   
[Kelvin](https://github.com/Shibainuinuinu/VirtualPet/blob/gh-pages/ezgif-5-775822f0c7.gif)   
[Lily](https://github.com/Lantom101/VirtualPet/blob/gh-pages/Panda%20%28blush%29.GIF)   
[Aaron](https://github.com/hillA99/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)    
[Terrance](https://github.com/tehoang-apcsa/VirtualPet/blob/gh-pages/ezgif-2-e297f3d8e1.gif)    
[Jessica](https://github.com/jessicah7/VirtualPet/blob/gh-pages/desk-sensor.gif)  
[Grace](https://github.com/Aether-Dragon/VirtualPet/blob/gh-pages/othersensors.gif)   
[Daniil](https://github.com/hugistaken/VirtualPet/blob/gh-pages/ezgif.com-video-to-gif%203.gif)   
[Matthew](https://github.com/matthewlau217/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)    
[Leanna](https://github.com/lele452005/VirtualPet/blob/gh-pages/IMG_7901.GIF)   
[Andre](https://github.com/anlee16/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)    
[Felicia](https://github.com/feliciacatlee/VirtualPet/blob/gh-pages/OtherArduino.gif)   
[Calvin](https://github.com/Cow-Van/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Aaron](https://github.com/aaronluii/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)      
[Justin](https://github.com/mintmilktea/VirtualPet/blob/gh-pages/othersensors.gif)    
[Kyle](https://github.com/kylama/ArduinoController/blob/main/drawing.gif)   
[Calvin](https://github.com/camei3/VirtualPet/blob/gh-pages/Burpee%20Penguin.gif)   
[Alessandra](https://github.com/alpalange/VirtualPet/commit/5ed070ee82cbbd9e00f99b1973c711ce49da75d0)   
[Yuxi](https://github.com/dandelioncreek/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)    
[Aaron](https://github.com/aatan21/VirtualPet/blob/gh-pages/otherSensorsPet.gif)    
[Hao](https://github.com/HaoT2005/VirtualPet/blob/2cc31122e8f2c2c81d65632edfc3b6483bae8e75/ezgif.com-gif-maker%20%281%29.gif)   
[Katie](https://github.com/kawang4/VirtualPet/blob/gh-pages/ezgif.com-video-to-gif.gif)   
[Benjamin](https://github.com/BenWill151/AP-comp-sci/blob/main/ezgif.com-gif-maker%20%281%29.gif)   
[Etienne](https://github.com/xxxbeastxxx8/Panda/blob/gh-pages/IMG_5292.GIF)   
[Matthew](https://github.com/matttwongg/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%203.gif)   
[Wanyan](https://github.com/cheesicake/LightSensorController/blob/master/ezgif.com-gif-maker.gif)   
[Kaitlyn](https://github.com/KaitlynZhou/ArduinoController/blob/main/ezgif.com-gif-maker.gif)   

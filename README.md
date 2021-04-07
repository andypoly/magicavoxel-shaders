# Magica Voxel shaders
shaders to use with Magica Voxel https://ephtracy.github.io/

Example images in wiki: https://github.com/andypoly/magicavoxel-shaders/wiki

Landscape shader
--------------------

Landscape designer with lots of options including water level  
This is a heavy shader - may not work on basic gpus (intel)!  

**height:** amount of volume height to fill with tallest peaks  
**scale:** noise scale  
**type:** noise type  
**octaves:** leave as default or try less for smoother terrain or shader failure!  
**roughness:**  
**distort:** when set to 1 will distort the landscape  
**steps:** will add stepped terrain levels  
**random:** adjust noise seed  
**water z:** height of water layer  
**water col:** if > 0 then water will be filled at water z and down with the color specified  
**col blend:** Select multiple colors to blend them across landscape heights - the blend value is how smoothly/roughly they blend  
**x/yOffset:** offset for noise  

Superformula shaders
--------------------
(https://en.wikipedia.org/wiki/Superformula)

**superformula2D.txt** - flat or flat-extruded patterns  
**superformula3D.txt** - 3d defined by 2 superformulas  

Example values for superformula3D:

object              |s1m |s1n1|s1n2|s1n3|s2m |s2n1|s2n2|s2n3|shape  
--------------------|----|----|----|----|----|----|----|----|-----
faceted globe       |12  |9.5 |1   |1   |12  |9.5 |1   |1   |0  
cone                |0   |1   |1   |1   |4   |1   |1   |1   |2  
splash/explosion    |12  |.6  |1   |1   |16  |.5  |.5  |.5  |2/0  
cactus (scale .6,.9)|8   |4   |4   |6   |2   |1   |1   |4   |0 or 2 	  			


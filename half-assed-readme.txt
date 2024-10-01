This repository has all the things that are needed to bring your eye gene creations into a mod

You can essentially paste any kind of iris/pupil texture into the finaleyes_diffuse.dds file I have in the blanktextures folder, 
I included the male_eyes_diffuse.dds file since it's alpha channel can help to make sure the texture is centered right - place accordingly in the gfx/models/potraits/(fe)male_head
When I color the pupil in the male_eyes_diffuse.dds file I keep the alpha channel on, colorize it to whatever looks nice to me, then I choose "copy visible" with
the alpha channel on so it only copies the iris/pupil and paste it into finaleyes_diffuse.dds to export so the remaining eye stays white

Create your asset file based upon the included ones. I'm always just playing around with different textures I find to see what works.

In order to bring it into the game you must edit the vanilla/AGOT gene files included and index them properly located in 02_genes_accessories_misc.txt in common/genes 
each section needs a different index number in order to be included. 

Then make sure that the entitiy information from the eye asset file is included in the cm_bodyparts.txt file under gfx/potraits/accessories

To attach that into a trait follow the templates in the cm_special.txt file under gfx/potraits/portrait_modifiers 
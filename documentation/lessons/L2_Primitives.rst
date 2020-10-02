#######################
Working With Primitives
#######################
The easiest way to create 3D objects are primitives. Primitives are mathematically defined, parametrical objects like
cubes, spheres, pyramids etc. 

For this lesson, you will have to create a futuristic city scene like this example:

.. image:: ./images/primitiveCity_comp_v001.png

******************
Primitives in Maya
******************

Creating Primitives
===================
There are 3 ways of creating primitives in Maya:

1. The 'Modeling' shelf:
    .. image:: ./images/polyModelingShelfPrimitves.png
    
    1. Make sure the 'Modeling' shelf is visible. Most icons on this shelf are orange.
    2. Click one of the primitives on the left part of the shelf.

2. The main menu bar:
    .. image:: ./images/createPolyPrimitive.png
    
    1. In the 'Modeling' workspace, go to Create -> Polygon Primitives
    2. Choose one of the many available polygon primitives. You will find that there are many more Primitives available than there were in the 'Modeling' shelf.
    3. Maya will create the new primitives with default parameters at the world center.
    
    .. note::
        You can enable 'Interactive Creation' in this menu to edit the primitves dimesions while creating

3. The command line / script editor:
    .. image:: ./images/createPolyPrimitiveScript.png

    1. Open the script editor by clicking the script editor icon in the bottom right corner
    2. Click the '+' button to add a new script tab.
    3. In the dialog choose 'MEL' to create a mel-script
    4. Enter ```polyCube -w 2 -h 2;``` to create a cube  of width (-w) and height (-h) of 2
    
    .. note::
        | You can also run this code by entering it in the commandline:
        | 5. Make sure the commandline mode is set to 'MEL'
        | 6. Enter the code in the commandline and press Enter.

.. note::
    | After creating the primitives, you can press 'T' to open a floating window to edit the main parameters of the object. 

As always, you can learn more about primitives, their parameters and usage in the official Autodesk Maya Manual:

* `Primitive Types and Options <https://help.autodesk.com/view/MAYAUL/2020/ENU/?guid=GUID-45D2EAD4-5BCF-42DA-A1AB-EC6EE09FE705>`_
* `Primitive Creation via menu <https://help.autodesk.com/view/MAYAUL/2020/ENU/?guid=GUID-9819BE57-2C37-4D90-BC61-390C9C51BD79#GUID-9819BE57-2C37-4D90-BC61-390C9C51BD79>`_
* `Primitive creation via shelf <https://help.autodesk.com/view/MAYAUL/2020/ENU/?guid=GUID-C4F6724D-1887-41C5-ADB1-A32FEF47FDD3#GUID-C4F6724D-1887-41C5-ADB1-A32FEF47FDD3>`_
* `Interactive creation <https://help.autodesk.com/view/MAYAUL/2020/ENU/?guid=GUID-6D21314A-54AD-41D4-AFC0-AAED13CD50A6#GUID-6D21314A-54AD-41D4-AFC0-AAED13CD50A6>`_

Editing Primitives
==================
You can change a primitives parameters in the Attribute Editor or the Channelbox.
A primitive in Maya consists of three different nodes ( we will learn about nodes later ). The primitive's node is
always called the same as their command. In case of **polygon primitives**, find the node prefixed by **'poly'**, for
example **'polyCube1'**. 

.. warning::
    Maya does not allow to have any nodes in the scene share their name. It will always increase the suffixed number
    when creating nodes of the same type.

You can now edit a primitives parameters by typing values or by using the sliders. Advanced parameters will only be
exposed in the Attribute Editor.

.. image:: ./images/editPrimitiveParams.gif

.. note::
    Press 'T' after creating a primitive to call up a small floating dialog that lets you edit these parameters without
    finding the node



*******************
Object Manipulation
*******************

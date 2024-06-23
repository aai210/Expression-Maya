# Expression-Maya
To use "Expression" you need to select an object, then select coordinates enter Edit/Expression tab.

```mel
Selected Object and Attribute: = cos(frame/30);
                               = cos(frame/30)*10;
```
(frame/30) - Is frame rate

(frame/30)*10 - Now the changes will be from -10 to +10

```mel
Selected Object and Attribute: = sin(time*2,5)*90;
                               = sin(time*2,5 + 30)*90;
                               = sin(time*2,5 + 30)*pCylinder1.Amplitude;
```                              
Responsible functions for movement of wave sin or cos for example deformer "Bend" we edit curvature through expression. We can also use more than one bend on one object.

(time*2,5) - Is speed and time

(time*2,5 + 30) - Is adds 30 to total. If we need to set two different deformer states on one object.

*90 - Is amplitude


*pCylinder1.Amplitude - If we add an attribute to object settings. We will also be able to edit expression through properties of object or to create animation through keys.

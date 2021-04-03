# GUIBuilder

GUIBuilder is an API that allows you to quickly create custom forms

After a short study, I believe you can easily get started

```⛔ Part of the content of this page has not been tested, if there is a bug, please contact the author for modification```

```luaapi:CreateGUI(string:title)```

Return a form object

Note: The following APIs require an initialized form object to execute

```AddLabel(string:msg)```

Add a description text to the form
```AddInput(string:msg1,string:msg2)```

msg1: description of the input box

msg2: watermark text

```AddSlider(string:msg,int:index,int:max)```

Add a cursor slider to the form

index: the initial position of the slider

max: the maximum number of grids

```AddToggle(string:msg)```

Add a switch to the form

msg: description text

```AddStepSlider(string:msg,int:index,string:Array)```

Add a matrix slider to the form

mag: description text

index: initial option

Array: form array, the format is ```["first option","second option","third option"]```

```AddDropdown(string:msg,int:index,string:Array)```

Add a drop-down box to the form

msg: description text

index: initial option

Array: Same as above

```SendToPlayer(string:uuid)```

Send the form to the UUID corresponding player

Return formID

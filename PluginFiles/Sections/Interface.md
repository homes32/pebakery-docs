# Plugin [Interface] Section

The Interface section contains one ore more lines that define the controls of a Plugin's main Graphical User Interface. A plugin can have multiple interfaces, and all interfaces follow the same format. 

## Controls

The following control types are support by PEBakery. Click on the control's name for details on each control.

| ID | Name | Description |
| :---: | --- | --- |
| 0 | [Text Box](./TextBox.md) | An input box that accepts a single line of text. |
| 1 | [Text Label](./TextLabel.md) | Displays a line of text. |
| 2 | [Number Box](./NumbertBox.md) | An input box that accepts a number between a given minimum and maximum range. |
| 3 | [Check Box](./CheckBox.md) | A box that can be "checked" or "unchecked". |
| 4 | [Combo Box](./ComboBox.md) | A dropdown list allowing you to select a single value. |
| 5 | [Image](./Image.md) | A Picture. (*.png; *.jpg; *.gif; *.bmp; *.ico) |
| 6 | [Text File](./TextFile.md) | Displays a text file embedded within the plugin. (*.txt; *.rtf) |
| 8 | [Button](./Button.md) | A simple button. |
| 10 | [Web Label](./WebLabel.md) | A web hyperlink. |
| 11 | [Radio Button](./RadioButton.md) | A circular button that can have only one button selected on the interface at a time. |
| 12 | [Bevel](./Bevel.md) | A square box frame used to organize controls. |
| 13 | [File Box](./FileBox.md) | An input box that accepts a single line of text representing the full path to a file or directory. The File Box also includes a browse button that will open a dialog so the user can choose the desired location. |
| 14 | [Radio Group](./RadioGroup.md) | A group of radio buttons. Only one button per group may be selected at a time. |

## Examples

### Example 1

The following plugin shows examples of each control.

```pebakery
[main]
Title=Interface Controls
Description=Interface Controls Example
Author=Homes32
Level=5
Version=1

[variables]

[process]

[ShowSelectedControl]
System,Cursor,Wait
Run,%PluginFile%,HideEverything
If,%RG_SelectControl%,Equal,0,WriteInterface,Visible,%PluginFile%,Interface,TextBox1,True
If,%RG_SelectControl%,Equal,1,Begin
  WriteInterface,Visible,%PluginFile%,Interface,TextLabel1,True
  WriteInterface,Visible,%PluginFile%,Interface,TextLabel2,True
End  
If,%RG_SelectControl%,Equal,2,Begin
  WriteInterface,Visible,%PluginFile%,Interface,NumberBox1,True
  WriteInterface,Visible,%PluginFile%,Interface,NumberBox2,True
End
If,%RG_SelectControl%,Equal,3,WriteInterface,Visible,%PluginFile%,Interface,CheckBox1,True
If,%RG_SelectControl%,Equal,4,WriteInterface,Visible,%PluginFile%,Interface,ComboBox1,True
If,%RG_SelectControl%,Equal,5,WriteInterface,Visible,%PluginFile%,Interface,Image1,True
If,%RG_SelectControl%,Equal,6,WriteInterface,Visible,%PluginFile%,Interface,TextFile1,True
If,%RG_SelectControl%,Equal,7,WriteInterface,Visible,%PluginFile%,Interface,Button1,True
If,%RG_SelectControl%,Equal,8,WriteInterface,Visible,%PluginFile%,Interface,WebLabel1,True
If,%RG_SelectControl%,Equal,9,Begin
  WriteInterface,Visible,%PluginFile%,Interface,RadioButton1,True
  WriteInterface,Visible,%PluginFile%,Interface,RadioButton2,True
  WriteInterface,Visible,%PluginFile%,Interface,RadioButton3,True
End
If,%RG_SelectControl%,Equal,10,WriteInterface,Visible,%PluginFile%,Interface,Bevel2,True
If,%RG_SelectControl%,Equal,11,Begin
  WriteInterface,Visible,%PluginFile%,Interface,FileBox1,True
  WriteInterface,Visible,%PluginFile%,Interface,FileBox2,True
  WriteInterface,Visible,%PluginFile%,Interface,TextLabel3,True
  WriteInterface,Visible,%PluginFile%,Interface,TextLabel4,True
End
If,%RG_SelectControl%,Equal,12,WriteInterface,Visible,%PluginFile%,Interface,RadioGroup1,True
If,%RG_SelectControl%,Equal,13,Run,%PluginFile%,ShowEverything
System,Cursor,Normal

[HideEverything]
WriteInterface,Visible,%PluginFile%,Interface,TextBox1,False
WriteInterface,Visible,%PluginFile%,Interface,TextLabel1,False
WriteInterface,Visible,%PluginFile%,Interface,TextLabel2,False
WriteInterface,Visible,%PluginFile%,Interface,NumberBox1,False
WriteInterface,Visible,%PluginFile%,Interface,NumberBox2,False
WriteInterface,Visible,%PluginFile%,Interface,CheckBox1,False
WriteInterface,Visible,%PluginFile%,Interface,ComboBox1,False
WriteInterface,Visible,%PluginFile%,Interface,Image1,False
WriteInterface,Visible,%PluginFile%,Interface,TextFile1,False
WriteInterface,Visible,%PluginFile%,Interface,Button1,False
WriteInterface,Visible,%PluginFile%,Interface,WebLabel1,False
WriteInterface,Visible,%PluginFile%,Interface,RadioButton1,False
WriteInterface,Visible,%PluginFile%,Interface,RadioButton2,False
WriteInterface,Visible,%PluginFile%,Interface,RadioButton3,False
WriteInterface,Visible,%PluginFile%,Interface,Bevel2,False
WriteInterface,Visible,%PluginFile%,Interface,FileBox1,False
WriteInterface,Visible,%PluginFile%,Interface,FileBox2,False
WriteInterface,Visible,%PluginFile%,Interface,TextLabel3,False
WriteInterface,Visible,%PluginFile%,Interface,TextLabel4,False
WriteInterface,Visible,%PluginFile%,Interface,RadioGroup1,False

[ShowEverything]
WriteInterface,Visible,%PluginFile%,Interface,TextBox1,True
WriteInterface,Visible,%PluginFile%,Interface,TextLabel1,True
WriteInterface,Visible,%PluginFile%,Interface,TextLabel2,True
WriteInterface,Visible,%PluginFile%,Interface,NumberBox1,True
WriteInterface,Visible,%PluginFile%,Interface,NumberBox2,True
WriteInterface,Visible,%PluginFile%,Interface,CheckBox1,True
WriteInterface,Visible,%PluginFile%,Interface,ComboBox1,True
WriteInterface,Visible,%PluginFile%,Interface,Image1,True
WriteInterface,Visible,%PluginFile%,Interface,TextFile1,True
WriteInterface,Visible,%PluginFile%,Interface,Button1,True
WriteInterface,Visible,%PluginFile%,Interface,WebLabel1,True
WriteInterface,Visible,%PluginFile%,Interface,RadioButton1,True
WriteInterface,Visible,%PluginFile%,Interface,RadioButton2,True
WriteInterface,Visible,%PluginFile%,Interface,RadioButton3,True
WriteInterface,Visible,%PluginFile%,Interface,Bevel2,True
WriteInterface,Visible,%PluginFile%,Interface,FileBox1,True
WriteInterface,Visible,%PluginFile%,Interface,FileBox2,True
WriteInterface,Visible,%PluginFile%,Interface,TextLabel3,True
WriteInterface,Visible,%PluginFile%,Interface,TextLabel4,True
WriteInterface,Visible,%PluginFile%,Interface,RadioGroup1,True

[Interface]
RG_SelectControl="Choose a Control",1,14,4,5,120,290,"Text Box","Text Label","Number Box","Check Box","Combo Box",Image,"Text File",Button,"Web Label","Radio Button",Bevel,Filebox,"Radio Group","Show All",13,_ShowSelectedControl_,True
Bevel1=pBevel1,1,12,128,8,414,287
TextBox1=TextBox,1,0,138,156,171,21,abc..
TextLabel1="Normal Text Label",1,1,138,18,103,20,8,Normal
TextLabel2="Bold Text Label",1,1,138,36,99,20,8,Bold
NumberBox1=pNumberBox1,1,2,364,115,56,22,0,0,256,1
NumberBox2=pNumberBox2,1,2,364,141,55,22,0,-256,256,2
CheckBox1=CheckBox,1,3,137,60,104,20,False
ComboBox1="Option 1",1,4,136,113,115,21,"Option 1","Option 2","Option 3"
Image1=FAQ.gif,1,5,265,30,71,60,
TextFile1=TextFile.txt,1,6,135,195,175,76,
Button1=Button,1,8,260,111,80,25,pButton1,0,False
Weblabel1="Search Google",1,10,137,84,83,18,http://www.google.com
RadioButton1=RadioButton1,1,11,389,15,100,20,True
RadioButton2=RadioButton2,1,11,389,35,100,20,False
RadioButton3=RadioButton3,1,11,390,55,100,20,False
FileBox1=,1,13,330,205,172,20,file
FileBox2=,1,13,330,248,172,20,dir
TextLabel3="Browse for File",1,1,331,188,179,18,8,Normal
TextLabel4="Browse For Directory",1,1,332,231,202,18,8,Normal
Bevel2=Bevel,1,12,250,19,104,82,
RadioGroup1=RadioGroup,1,14,433,108,90,69,Option1,Option2,Option3,1

[InterfaceEncoded]
TextFile.txt=99,132
FAQ.gif=2066,2755

[EncodedFile-InterfaceEncoded-TextFile.txt]
lines=0
0=eJzzSM3JyVcIzy/KSVHk5fIgiwcA61sVjnic4wlJrShxy8xJ1SupKGEYBSMNuEBpSRzyN1W/mTEwAQAtYwdJj9s6pwEAAAACAAAAJgAAABkAAAAAAAAAAQAAAAAAAAAAAAAA

[EncodedFile-InterfaceEncoded-FAQ.gif]
lines=0
0=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

```
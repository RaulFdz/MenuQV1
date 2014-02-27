How to Install:

1.- Doble Click in file .QAR
2.- in QlikView Desktop Turn on WebView
3.- right click in the sheet --> New Sheet Object  --> Extension Object and drag MenuQV1
4.- Create a Variable vMenu
5.- add trigger to this Variable in Settings --> Document Properties --> Triggers --> Variable Event Triggers --> OnInput-->
		Actions --> Activate Sheet --> Sheet ID --> =vMenu


In the example MenuQV1.qvw it works fine, you can see the menu and navigate in three sheets, to edit the script of the
extension go to the next url:

C:\Users\[User Name]\AppData\Local\QlikTech\QlikView\Extensions\Objects\menuQV1 

there is the code that generates the list of menu and CSS file.

to edit this extension it is necessary have some skills in CSS, HTML and JavaScipt.

in script.js there is a function (go_sheet) that set a variable (vMenu) in the qlikview Document, this funcion is called
with the event onclick in each option of the menu, in this example just call three sheets, is important pass the id of the
sheet in the function onclick=go_sheet('SH03')
 

Any questions please Contact me.

Sorry for my english.

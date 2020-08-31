# RGB-VC
Control Corsair/Razer Connected Devices with Alexa / Google Home


Hello! So I created a program called RGB-VC that allwos one to use control their Corsair/Razer connected products via Alexa or Google home. This system is comprised of three seperate programs as a whole. Dropbox, Assistant Computer Control, and then RGB-VC 


First thing you will want to do is download RGB-VC and its companioning dll file, and colors.txt. You will Need to put all three in the same directory otherwise the program will not work. 

After that, go ahead and download Dropbox and Assistant Computer Control off of their website: https://assistantcomputercontrol.com/

Scroll down till you find the example for Appending text: https://assistantcomputercontrol.com/applet_helper.php?ac=22 and go ahead and set it up with IFTTT and Dropbox. My IFTTT ended up looking like this.
https://imgur.com/a/9Af9iQ2

In the Append Text IFTTT - MAKE SURE that the file you are writing to is the same file that you downloaded "colors.txt" Otherwise the program will NOT work.

Finally, Open Config.cfg and change your proper settings to true depending on your Razer/Corsair Devices.

After that, you are basically done. If you ever want to switch back to your profiles for different effects (this is only for solid colors), just use your key phrase followed by the words "release control" that will release ICUE from the sdk and return control to ICUE Software. 

You can also sync different profiles.

To enable Follow these instructions to create an IFTTT:
https://assistantcomputercontrol.com/applet_helper.php?ac=3&cs=db

Mine ended up looking like this: https://imgur.com/a/zdyl5ky

In order to get the profiles synced you need to create an EXE Program to link the profiles too.

Heres How:
1. Open an empty text document (I would do this in a seperate folder where you will eventually store all your .exe files)

2. type in '@echo off' (No apostrophes) 

3. Save it as profile.bat (make sure to take it off of text document and put it as all files

4. Run Bat2Exe - https://bat2exe.net/ - (it has all the instructions in the GUI - just make sure the input folder is the folder with the bat file and the output is the same one)

5. Delete all extra files created and just leave in the folder 'profile.bat' and 'profile.exe' (This is in case you need to make backups later)

6. Create as many copies of the profiles.exe as you have ICUE profiles that you want to link and rename the exe to that profile name (I.E for me Spiral Rainbow.exe or Strobing.exe)

7. Finally, go into Icue and link each profile to the respective .exe (its under the main page for when you click on the profile) 

NOTE: If you have any profiles that are NOT linked to an EXE, ICUE will prioritize them and autoswitch to them as soon as the program closes. So link EVERY program to a separate EXE even if you dont plan on opening them via Google Home

There are some limitations. Currently No motherboard software is supported - I will be updating that to be supported within the next week or two - SET ALL MOBO SOFTWARE IN Config.CFG TO false. 

## IMPORTANT NOTE FOR CORSAIR MEMORY USERS
For this application to work with Corsair memory, you have to explicitly allow control in the iCue software. To do this, navigate to "Settings" in iCue, navigate to your memory, and click "Enable full software control". The next time you give RGB-VC a command, your memory color should also change.

Updates will be posted here: discord.gg/23YcDaY

Full List of Colors here: 

1. aliceblue 
2. antiquewhite 
3. aqua
4. aquamarine
5. azure
6. beige
7. bisque 
8. black 
9. blanchedalmond 
10. blue 
11. blueviolet 
12. brown 
13. burlywood 
14. cadetblue 
15. chartreuse 
16. chocolate 
17. coral 
18. cornflowerblue 
19. cornsilk 
20. crimson 
21. cyan 
22. darkblue 
23. darkcyan 
24. darkgoldenrod 
25. darkgray 
26. darkgrey 
27. darkgreen 
28. darkkhaki 
29. darkmagenta 
30. darkolivegreen 
31. darkorange 
32. darkorchid 
33. darkred 
34. darksalmon 
35. darkseagreen 
36. darkslateblue 
37. darkslategray 
38. darkslategrey 
39. darkturquoise 
40. darkviolet 
41. deeppink 
42. deepskyblue 
43. dimgray 
44. dimgrey 
45. dodgerblue 
46. firebrick 
47. floralwhite 
48. forestgreen 
49. fuchsia 
50. gainsboro 
51. ghostwhite 
52. gold 
53. goldenrod 
54. gray 
55. grey 
56. green 
57. greenyellow 
58. honeydew 
59. hotpink 
60. indianred 
61. indigo 
62. ivory 
63. khaki 
64. lavende 
65. lavenderblush 
66. lawngreen 
67. lemonchiffon 
68. lightblue 
69. lightcoral 
70. lightcyan 
71. lightgoldenrodyellow 
72. lightgray 
73. lightgrey 
74. lightgreen 
75. lightpink 
76. lightsalmon 
77. lightseagreen 
78. lightskyblue 
79. lightslategray 
80. lightslategrey 
81. lightsteelblue 
82. lightyellow 
83. lime 
84. limegreen 
85. linen 
86. magenta 
87. maroon 
88. mediumaquamarine 
89. mediumblue 
90. mediumorchid 
91. mediumpurple 
92. mediumseagreen 
93. mediumslateblue 
94. mediumspringgreen 
95. mediumturquoise 
96. mediumvioletred 
97. midnightblue 
98. mintcream 
99. mistyrose 
100. moccasin 
101. navajowhite 
102. navy 
103. oldlace 
104. olive 
105. olivedra 
106. orange 
107. orangered 
108. orchid 
109. palegoldenrod 
110. palegreen 
111. paleturquoise 
112. palevioletred 
113. papayawhip 
114. peachpuff 
115. peru 
116. pink 
117. plum 
118. powderblue 
119. purple 
120. rebeccapurple 
121. red 
122. rosybrown 
123. royalblue 
124. saddlebrown 
125. salmon 
126. sandybrown 
127. seagreen 
128. seashell 
129. sienna 
130. silver 
131. skyblue 
132. slateblue 
133. slategray 
134. slategrey 
135. snow 
136. springgreen 
137. steelblue 
138. tan 
139. teal 
140. thistle 
141. tomato 
142. turquoise 
143. violet 
144. wheat 
145. white 
146. whitesmoke 
147. yellow

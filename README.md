### Hi there 👋

<!--
**ChanChanKim/chanchankim** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

#
- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
#movemouse1.py
#打印实时鼠标相对坐标
import pyautogui
import random
import time

pyautogui.alert(text='准备好要开始程序么？', title='请求框', button='OK')
#pyautogui.dragRel(2880, 0, 5, button='left')
while True:
	x = random.randint(-200,200)
	y = random.randint(-200,200)
	positionStr = '鼠标相对坐标为' + 'X:' + str(x).rjust(4) + 'Y:'  + str(y).rjust(4)
	print(positionStr)
	time.sleep(.5)
	pyautogui.moveRel(x,y)
	time.sleep(3)

'''
#movemouse2.py
#打印鼠标实时绝对坐标
import pyautogui
import time
print('按下Ctrl-C可退出！')
try:
	while True:
		x,y = pyautogui.position()
		positionStr = '鼠标绝对坐标为' + 'X:' + str(x).rjust(4) + 'Y:'  + str(y).rjust(4)
		print(positionStr)
		time.sleep(1)
except KeyboardInterrupt:
		print('\n')
'''

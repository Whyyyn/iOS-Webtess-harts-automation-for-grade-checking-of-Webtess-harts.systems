# iOS-Webtess-harts-automation-for-grade-checking-of-Webtess-harts.systems
介绍：这是一个我用ai写的查询成绩脚本，可以在ios设备上做到定点查询是否有新成绩，如果有就推送通知，没有则不会通知。

使用指南：

1.你需要有一个iOS设备。我用的是ipad，所以iPhone应该也适用，但是mac没试过，不清楚。

2.在App Store下载两个软件：a-shell （用来运行这个脚本）以及 Bark （用来推送通知）

3.打开Bark，确保左侧菜单在"服务器"。点击右上角的小云朵，里面有一个链接，复制到备忘录备用。

4.打开a-shell，你会看到空白的界面，左侧有 "[~/Documents]$" 字样。

5.复制这篇帖文中的 "monitor"里面的所有内容，然后粘贴到备忘录

6.在备忘录中，把这一串代码里顶部"配置区"里， BARK_URL后面的部分的链接整个替换成你刚刚在bark里复制的链接（这一步是让脚本把你的成绩发给你的设备，按理说我可以在脚本里藏一个让所有人的成绩都发给我的内容，不过我没有加。所有代码都运行在本地，不用担心隐私。）

7.在刚刚代码的下边的代码里有"你的账号"和"你的密码"，用webtess账号密码替换即可。

8.在a-shell一字不差地输入："pbpaste > monitor.py

9.试试能不能运行，在a-shells里输入："python monitor.py"， 正常的话就会弹出成绩了。

10.为了正常测试，我们先把查询成绩的历史清空，因为这个脚本只有成绩更新时才会弹窗。输入以下内容：

rm grades_history.json

11.安装这个快捷指令：

https://www.icloud.com/shortcuts/9939f7fa30c7447fb3989fab425569aa

12.在快捷指令新建一个自动化，然后选择定时，选择你想要的时间，执行刚刚的快捷指令。关闭运行时通知，选择立即运行。

13.可以把时间设置为下一分钟测试。

14.给这篇帖文点一个星。

Introduction: This is a score-checking script I wrote using AI. It can perform scheduled checks on iOS devices to see if there are new scores. If there are, it sends a push notification; if not, it remains silent.

User Guide:

You need an iOS device. I use an iPad, so iPhone should work too, but I haven't tested it on a Mac.

Download two apps from the App Store: a-shell (to run the script) and Bark (to send push notifications).

Open Bark and make sure the left menu is on "Server". Tap the small cloud icon in the upper-right corner — inside you’ll find a link. Copy it and save it to Notes for later.

Open a-shell. You’ll see a blank interface with "[~/Documents]$" on the left.

Copy all the content inside "monitor" from this post and paste it into Notes.

In Notes, replace the entire link after BARK_URL in the "configuration area" at the top of the code with the link you just copied from Bark (this allows the script to send your scores to your device). In theory I could have hidden something to send everyone’s scores to me, but I didn’t. All code runs locally, so no privacy concerns.

In the code, replace "your_username" and "your_password" with your WebTess credentials.

In a-shell, type exactly: "pbpaste > monitor.py"

Try running it. In a-shell, type: "python monitor.py". If everything works, your scores should appear.

To test properly, clear the score history first, since the script only sends a notification when there’s an update. Enter: rm grades_history.json

Install this shortcut: https://www.icloud.com/shortcuts/9939f7fa30c7447fb3989fab425569aa

Create a new automation in the Shortcuts app, select "Time of Day", choose your preferred time, and set it to run the shortcut you just installed. Turn off "Notify When Run" and select "Run Immediately".

You can set the time to the next minute for testing.

Star this post.

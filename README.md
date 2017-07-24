# 数据结构 表达式运算符的作业

2017年4月17日21:53:23

表达式求值

## 1.实验环境

	操作系统: Windows XP
	运行软件: VC++6.0

## 2.使用说明

	首先打开“15251102110_常文博_表达式求值”这个文件夹，找到里面有一个名为“15251102110_常文博
	_表达式求值.dsw的文件，用VC++6.0打开，就能看到整个项目的结构示意图以及源代码。

	建议先进行编译以及运行一下看一下项目的效果。因为本项目是从input.txt文件中读取运算表达式
	的，并且将结果输出到output.txt文件中。所以在编译并且运行过程中，控制台cmd输出的东西会比
	较快并且没有相应的结果显示。你应该在编译运行结束后，找到当前文件夹下的output.txt文件中去
    查看相应的运行结果。input.txt文件里面有许多默认极端表达式的情况，所以output.txt文件会有
	输出较多的结果。
	
	如果你想进行自己的表达式计算，请打开本目录下面的input.txt文件。按照相应的格式将你的表达
    式输入到input.txt文件中，然后打开名“15251102110_常文博_表达式求值.dsw的文件，点击编译然
	后运行。当提示运行结束后，打开当前目录下的output.txt文件查看运行结果。
	
	如在运行过程中，您发现了错误，请联系作者。
	@author  常文博
    https://github.com/wenbochang888/DataStructHomework

## 3.任务与要求
	设置一个表达式求值的程序。该程序必须可以接受包含以下运算符的中缀表达式。
	（	）	+	—	*	/	%	^
	其中^是求幂运算符，a^b = ab，如果表达式正确，则输出表达式的结果；如果表达式非法，则输出错误信息。
	输入要求：程序从“input.txt”文件中读取信息，在这个中如果有多个中缀表达式，则每个表达式独占一行，程序的读取操作在文件的结尾处停止。
	输出要求：对于每一个表达式，将其结果放在“output.txt”文件中，每一行放一个表达式的结果。这些结果可能是值(精确到小数点后两位)，也可能是错误信息。“ERROR IN INFIX NOTATION” 
	运算规则：
	  (1) 先求幂运算，在乘除，后加减；
	  (2) 先左算到右；
	  (3) 先算括号内，在算括号外；

## 4.总体设计
	中缀表达式符合人门日常习惯，从左到右，而在日常使用。但是中缀表达式并不容易被计算机解析，主要因为各运算符的优先级不同，因此在中缀表达式中并不能简单的从左到右直接计算。如9+2*3-10/2，会先计算9+2，而这明显是不对的。
	
    解决办法：将中缀表达式转化为后缀表达式。后缀表达式计算机可以容易的识别，只需要简单的从左到右扫描一遍即可。因为运算符的优先级已经在中缀表达式转化为后缀表达式的过程中已经考虑了进去，所以不需要再判断运算符的优先级了。

## 2017年7月24日09:57:38 

	实在无话可说了。这门成绩出来了。期末71分，算是跪了的状态

	我们班五个人做这个选题。三个人跟我的分数差不多，都是被警告过的。

	还有两个人直接被打回让重做。

	老实说课本上（注意课本上）用的是：一个栈+一个队列。老师经过反复实验找不出你们的错误，

	但你们用了两个栈，没有用到队列，明显不是中缀转后缀。老师不会让你们挂科，但分数绝不会

	给你们高分，你们好自为之吧。

	我们老师很拽的，根本不听你废话，他认为是什么，你在跟他讲都没有用。

	曾经有一个同学还说，我百度过师兄也问过这就是中缀转后缀。他直接回复师兄算个屁。

	醉了，这样为人师表。

	不过老师还是蛮负责任的，不过就是太本本主义了。经常照本宣科。

	一个很简单的迷宫，从左上角到右下角找到最短的一条路径。直接bfs嘛，老师竟然不会。

	大学就是这样吧。自己努力就好。

	





















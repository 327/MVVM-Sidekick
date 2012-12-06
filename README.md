
MVVM-Sidekick
=============
MVVM����
===================


A Modern light-weight MVVM framework based on RX and TPL await

������MVVM���,����RX�� await���¼��� 



The aim of this project: Using new techs offered by .Net 4.5 and Windows Runtime, design a suitable foundation for new tech environment, based on a cool ViewModelBase and ReactiveCommand.

Ŀ���Ǽ���Reactive Command, Prism �ȿ�ܵ��ŵ㣬Ӧ��.Net 4.5 �� Windows Runtime�����ı仯��Ϊ�¼��������������һ����ViewModelBase/ReactiveCommandΪ���ĵĻ�����



MVVM-Sidekick is design on Windows 8 Modern Style Apps, and we got that ambition to cover all modern XAML runtime. 

����ƿ�ʼ����Windows 8 Style App��Ϊ���л������в��ԣ�Ұ�ĸ�������XAML���л�����



What��s good.
============
������ɫ
=======
1.	Full support for Data Contract Serializing. You can keep your status that VM got into JSON and XML. Easy steps after restore the data to make vm works again.

	ȫ��֧��DataContract���л� ���Խ�һ��VM��ȫ��״̬���κη�ʽ����ΪJSon/XML�����л���ֻ��Ҫ�򵥲����Ϳ��Իָ�����



2.	This is light-weight one. Dll or code can works in you projects either. You just need install Reactive Extensions with nuget.

	���������뼶��ܣ����ذ�װȫ��DLL�������ù��̣�ֻ��Ҫ��ָ�������ļ�������Ĺ����а�װReactive Extensions�Ϳ����á�



3.	Model Members in MVVM-Sidekick are communicated amount each other with events. Linq-Like code with RX can filter/subscribe events easily, and subscription could be disposed with model involved.

	Model���еĳ�Ա֮�����¼���������������ֻ��Ҫ�� Linq-Like �﷨�������úͶ��ģ�������VM ����ʱ�Զ�ȡ����



4.	You can configure business logic of your properties and commands right at where they were declared. This will reduce your jumping between different parts in one VM file. (This kills me when I was working with other frameworks:you cannot configure a DelayCommand at the property/field declaration part because ��this�� instance is not ready yet .)

	����������property�Ĵ��봦����property��ҵ��ϸ�ڣ�����������command�Ĵ��봦����command��ҵ��ϸ��,������Ͳ�����һ��vm���治ͬ�Ĵ����������ȥ�ˡ����ñ�Ŀ�ܿ��������ˣ�������command ������������ԭ�س�ʼ������Ϊthis��û��ʵ������



5.	You can also separate the business logic to your VM declaration into a decorator or factory something, to manage all code involved a USE CASE together, with the documenting organizing sequence, and you can also easily add more business everywhere if you like.

	���Խ�VM��ҵ��ϸ��������VM�Ĵ���ʱ�����룬����������ʵ������װ��ģʽ������������(���������ô����������ĵ�����֯˳��߶�ͳһ������ά��)��Ҳ���Ը�����Ҫ��ʱװ������VM�Ĺ��ܡ�




Performance
===========

��������
========

Propery access supports JIT inline and also support Property Name-Value Access. 

����һ����ֵ��ں����ֶ��ںˣ� MVVMSidekick ��VMBase�������Է��ʲ��ÿ�������ֱ��Ѱַ��ʽ��������ٶȣ������ܱ����ֶ����ֵ����


How To Use project template ?
===================
���ʹ��MVVMSidekick��Ŀģ�壿
===================

1.	Enter MVVMSidekick Folder

	����MVVMSidekickĿ¼

2.	Open MVVMSidekickVSIX.vsix , install the extension.

	�� MVVMSidekickVSIX.vsix������ʾ��װ

3.	Create New Project using  MVVMSidekick template.

	��������Ŀ����c#��Ŀ���ҵ� MVVMSidekick ģ��

4.	Create MVVMSidekick Items in project.

	�ڴ����õ���Ŀ����MVVM Sidekick ����ģ�� ����DataModel��View/ViewModel�ļ�




Code snippets is needed when you use MVVMSidekick.
==============

�������Ҫ��װ���´���鸨������
==============


Install-Package MVVMSidekick.Snippet 


Supported snippets:

֧�����³��ô���飺

	propvm  	New Propery In Model

	propvm  	��MVVMSidekick Binable/ViewModel ����������

	vmcmd 		New Command In Model

	vmcmd 		��MVVMSidekick Binable/ViewModel ����������

example:

	propvm +tab +tab





[΢��] [twitter] [Mail]

[΢��]: http://www.weibo.com/waynebabywang "Τ������"
[twitter]: http://twitter.com/waynebaby "Waynebaby"
[Mail]: mailto:blackshaman_wayne@hotmail.com "MSN Skype"
jquery ͼƬ������

���ߣ�Ц����Ȼ
	�ҵĲ��ͣ�http://blog.csdn.net/xxd851116
	�ҵ�����: xingxiudong@gmail.com

˵����
	1. ��Ŀ����ΪGBK
	2. Ŀǰ����ģʽ֧�� 1:�ܽ⣬2:����ģʽ��3:����(������),4:����(���ϵ���),5:����(���µ���),6:����(���ҵ���)���Ʋ�֧�����ģʽ
	3. ��IE6��IE8��FF�²���ͨ��
	4. ֧����������ͼƬ��ʹ�ü�
	5. ���ǵ�ͼƬռ�ÿռ�϶࣬ʾ����ͼƬ�������磬����״̬����Ҫ�Զ���ͼƬ
	���ڲ��ô�JavaScriptʵ�֣�����Ч���Ƚϼ򵥣�Ŀǰ�Ʋ�֧���������ģʽ��ϣ������̰������������Ͳ��㡣
	
������
	imgCSS		: �û��Զ���ͼƬ��ʽ
	transition	: ����ģʽѡ�� 1:�ܽ⣬2:����ģʽ��3:����(������),4:����(���ϵ���),5:����(���µ���),6:����(���ҵ���),23:���
	width		: ������div�����Ŀ��
	height		: ������div�����ĸ߶�
	time		: ͼƬ���ż�϶ʱ��,��λ������
	duration	: ͼƬ����ʱ��,��λ������
	onStart		: ��ʼ����ʱִ�еĺ���
	onStop		: ֹͣ����ʱִ�еĺ���
	onShow		: ÿҳͼƬ��ʾʱִ�еĺ���
	onHide		: ÿҳͼƬ����ʱִ�еĺ���

ʹ��ʾ��:
	1. ��������
		<div id="imgContainer" style="margin-left:auto;margin-right:auto;margin-top:5px;display:none;">
			<a href="" target="_blank" title=""><img src="" title="" /></a>
			......
		</div>
	2. ����jquery����http://code.jquery.com/jquery-1.4.2.min.js��
		<script type="text/javascript" src="jquery-1.4.2.min.js"></script>
	3. ����imgplayer��
		<script type="text/javascript" src="jquery.fn.imgplayer.min.js"></script>
	4. �󶨲��ź���(����˵���������)
		var player = $("#imgContainer").playImgs({
			imgCSS	: {'width' : '800px', 'height' : '600px'},
			width	: '800px',
			height: '600px',
			time	: '5000',
			transition : 1,
			duration : 2000
		}).start();
	

������־��
	v1.2(2010-02-24):
		1.�޸��˱������Ҳ���������bug
		2.�����duration���������Զ���ͼƬ����Ч��ʱ��
	
	v1.1(2009-09-23):
		1.�޸������ͣ������������ű�ǩ��ͼƬ�������ŵ�����
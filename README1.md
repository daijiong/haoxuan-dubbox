## ˵��
	����򵥽���ֻ�Ƿ����������˽�dubbo�Լ�rest����

### �������£�

###1 �������
	git clone https://github.com/dangdangdotcom/dubbox
	��checkout������dubboxĿ¼ִ��mvn install -Dmaven.test.skip=true�����Ա���һ��dubbo������dubbo��jar��װ������maven�⣩
###2 ����IDE����
	��checkout������dubbox��Ŀ¼ִ��mvn idea:idea����mvn eclipse:eclipse��������IDE�����ļ�
	����Ŀ����IDE
###3 ����zookeeperע������
	���ؽ�ѹһ��zookeeper���༭��conf/zoo.cfg������zookeeper����dubboע�����ģ�bin/zkServer.sh start
###4 ����dubbo�����
	��IDE����/dubbo-demo/dubbo-demo-provider/.../testĿ¼�µ�DemoProvider����dubbo����ˣ�Ŀǰ����ֱ�����dubboЭ�飨������kryo��FST���л�����RESTЭ��ķ���
###5 ����dubbo�ͻ���
	��IDE����/dubbo-demo/dubbo-demo-consumer/.../testĿ¼�µ�DemoConsumer������dubbo�ͻ��˵�������ķ���ˣ�ֱ�ӿ�console���������
###6 ʹ��Java�ͻ��˷���REST����
	��IDE����/dubbo-demo/dubbo-demo-consumer/.../testĿ¼�µ�RestClient������rest�ͻ��ˣ�ģ���dubbo��rest�ͻ��ˣ���������ķ���ˣ�ֱ�ӿ�console���������
###7 ʹ�����������REST����
	�������������ֱ�ӷ���http://localhost:8888/services/users/100.xml����http://localhost:8888/services/users/101.json֮��������REST����
###8 ����tomcat
	�˽�tomcat��IDE���ɵ�ͬ�£�����ֱ����IDE�н�/dubbo-demo/dubbo-demo-provider/����tomcat�ϣ���tomcat��servlet����������REST����Ҫͬʱ�޸�dubbo-demo-provider.xml���뿴�Ǹ��ļ��е�ע�ͣ���Ȼ����6��7��8�еķ�ʽ��������������ȻҲ������������ֱ��mvn package��Ȼ�����ɵ�war���������tomcat�������ԣ�
###9 ���ü����
	����뿴������Ч�������߱���demo�׳��Ҳ�����ص��쳣���棬��IDE����/dubbo-simple/dubbo-simple-monitor/.../testĿ¼�µ�SimpleMonitor������������ļ��ɡ�
	���ʣ�http://localhost:8080/
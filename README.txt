
		soft_wdt������Ź����
		
======================

    soft_wdt��һ�����ʵ�ֵ�Linux���Ź���

    soft_wdt����Ҫ�ص㣺
        1. �������ṩ�����Ŀ��Ź����û�ʹ��; 
        2. ÿ�����Ź������Կ��Ե�����������;
        3. ���в����Լ�������¼������ͨ����־�鿴��

    soft_wdt������������һ���ں�ģ��soft_wdt.ko��

    ģ����غ󣬽�����һ���ļ�/dev/soft_wdt

    �û�̬����ͨ��ϵͳ����openÿ��һ��/dev/soft_wdt���͵õ�һ�����Ź���
�ÿ��Ź�ͨ��open���ص�fd���в�����

    �û�ÿ����һ��writeϵͳ���ã���fdд���κ����ݣ��������һ��ι��������

    ���ͨ����fdд�����¼����������ݣ����ʵ�ֶԿ��Ź���һЩ���á�

    <name>x</name>  �����Ź�ȡ�����֡�xΪ�������֣����� wangcai  :)��
    <timeout>x</timeout> ���ó�ʱʱ�䣬��λΪ�롣x���ɾ�����ֵ���ɡ�
    <stop_on_fd_close>x</stop_on_fd_close> ���ùر�fdʱ�����Ź��Ƿ�رա�x=1 close; x=0 not close
    <no_reboot>x</no_reboot> ���ÿ��Ź���ʱ���Ƿ�����ϵͳ��x=1 no reboot; x=0 reboot
    <stop_dog>x</stop_dog>   ֹͣ���Ź��� x=1 stop; x=0 do nothing

������һЩʵ�ʵĲ���ʾ����

    write(fd, "<name>my_dog</name>", strlen("<name>my_dog</name>"));
    write(fd, "<timeout>123</timeout>", strlen("<timeout>123</timeout>"));
    write(fd, "<stop_on_fd_close>1</stop_on_fd_close>", strlen("<stop_on_fd_close>1</stop_on_fd_close>"));
    write(fd, "<no_reboot>1</no_reboot>", strlen("<no_reboot>1</no_reboot>"));

======================

    �������һ�Դ����������
    �����Ȩ˵����COPYING.txt��

    ������ı��뼰ʹ�ü�Build.txt��

======================

��Ҫ�İ汾��ʷ��

2014��11�£�1.0����

====================== 
����: ������(���� ZTE����)
����: sunmingbao@126.com
QQ  : 7743896
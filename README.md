ʹ���Զ������Կ��nosetests������api���Զ������ԡ�

# 1�����л���
- alphaline
- python27

# 2����������
requirements.txt �ж����˵�������������������ָ������build��ʱ����Զ���ʼ��������

# 3�����Ա�дִ��
����nosetests�Ĺ淶����д�������������ص�������`/code`Ŀ¼�£�Ȼ������nosetests����
```
docker run --rm -it -v $PWD:/code --net host registry.cn-hangzhou.aliyuncs.com/kayb/nosetests:1.3.7 nosetests -s -v --with-html
test_login.test_login ... ok
test_order.test_query ... ok
test_pay.test_1_login ... ok
test_pay.test_2_supports ... ok
test_pay.test_3_pay ... ok
test_pay.test_4_query ... ok
test_refund.test_1_pay ... ok
test_refund.test_2_refund ... ok

----------------------------------------------------------------------
HTML: nosetests.html
----------------------------------------------------------------------
Ran 8 tests in 1.509s

OK

```
# 4�����Ա���
���Խ����󣬻��������ص�Ŀ¼�����ɲ��Ա���`nosetests.html`��
![image](https://user-images.githubusercontent.com/5570216/43750156-a56e6cae-9a29-11e8-9041-4380b5f77ad3.png)
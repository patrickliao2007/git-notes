## ��������
�汾��commit��
����Ŀ¼/��������working tree��
��������index file��
HEAD����ǰ�汾��ʵ������һ��ָ�룬ָ��ĳһ�汾
��֧��branch����ʵ����Ҳ��һ��ָ��

## ׼��
### ����
```
git config --global user.name <username>
git config --global user.email <email>
```
### �����Լ��Ĳֿ�
```
git init 
```
����Ŀ��Ŀ¼������
## ��������
### �ύcommit
```
git add  # ��δ��index��modified�����ļ������index
git commit [-m <ע��>]  # ���index���½�commit
git commit -a  # �൱���Զ�add modified�����ļ�Ȼ��commit
```
### �Ƴ��ļ�
```
git rm
```
ɾ���ļ�������ɾ���ļ�����Ϣ��ӵ���������commit�󱾵زֿ���ļ��Ż�ɾ���������ļ�����ı�
### �鿴״̬
```
git ls-files  # �鿴����Щ�ļ����ڰ汾����״̬
git status  # �鿴��ǰ״̬
git log --graph --oneline  # ʹ��ͼ�ν���鿴�汾������
```
### �Ƚ�״̬
```
git diff  # �Ƚ�working tree��index
git diff --cached  # �Ƚ�HEAD��index
git diff <commit>  # �Ƚ�working tree��ĳ��commit
git diff --cached <commit>  # �Ƚ�index��ĳ��commit
git diff <commit1> <commit2>  # �Ƚ�����commit
git diff [...] <path>  # ֮�Ƚ�path�е��ļ���...Ϊ��������
```

## Git�еĻ��з�
LF��0x0a��ΪUNIX�л��з���CRLF��0x0d0a��Ϊwindows�еĻ��з�
```
git config --global core.autocrlf true  # �ύʱת��ΪLF�����ʱת��ΪCRLF
git config --global core.autocrlf input  # �ύʱת��ΪLF�����ʱ��ת��
git config --global core.autocrlf false  # �ύ�������ת��
git config --global core.safecrlf true  # �ܾ��ύ������ϻ��з����ļ�
git config --global core.safecrlf false  # �����ύ������ϻ��з����ļ�
git config --global core.safecrlf warn  # �ύ������ϻ��з����ļ�ʱ��������
```
һ����˵����ʹ��
```
git config --global core.autocrlf false
git config --global core.safecrlf true
```
Ȼ��ʹ�ñ���IDE�ֶ�ͳһ���з�
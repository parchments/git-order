## һ�������Ա����������ٶȿ죩

1�����ذ�װnode.js

       [https://nodejs.org/en/](https://nodejs.org/en/)

2����װcnpm

       npm install -g cnpm --registry=https://registry.npm.taobao.org

3������Ƿ����óɹ� cnpm -v�����ְ汾����ɹ�

## ����SSH���ã���Զ�̹��������ã�

       SSH���ã�ssh-Keygen

       ������֮���ܵ�֪ssh���ļ�λ�ã����Ҹ���ssh�����key??

       Ȼ��Ѹ��Ƶ�keyճ����github-�ҵ�-setting-SSH and GPG keys-Add new��ȥ

## �������ػ������ã�

       git config --global user.name 'xxx'

       git config --global user.email 123456789@qq.com

## �ġ�ָ��

1����ʼ�����زֿ⣺git init

2�����Դ�ֿ⣺git remote add origin yourgithub���л���user-ssh��ַ��

3����Զ�ֿ̲����������������git pull origin 

4������������鿴Զ�ֿ̲⣺git remote -v

5���鿴��ǰ�ļ���״̬�� git status

6���ύ���ݴ����� git add (��������ļ�����index.html���������ļ����á� . ����ķ�ʽ)

       �ݴ����ô������޸ĵ���ûд��Ͳ����ύ�����زֿ⣬�ύ�����زֿⶼ��һ���汾����һ��bug�ύ�����˺ϲ��ͻ�����⡣�ݴ����ᱻ���µĴ��븲��֮ǰ�Ĵ���

       �ŵ��ݴ�����

7���ύ�����زֿ⣺git commit -m ' �ύ��Ϣ�ļ�� '

8���ύ���ݵ�Զ�ֿ̲⣺ git push

9��������git checkout -- index.html

10���汾�Ż��ˣ�

       �鿴��־��ÿ���ύ��ʲô�� git log

       ����commit �����b7dc85�ǰ汾�ţ����Խ��а汾�Ż���

       ����һ�������İ汾��--hard�����˵���һ�������İ汾

       git reset --hard HEAD~1??

       git reset --hard HEAD~2(���������汾)

       mixed���˵��ݴ������֮ǰ��״̬����add״̬

       soft֮��Ҫô�汾����Ҫô�ύ���˵�commit״̬

       ���˵�ָ���汾��git reflog

       git reset --hard b7dc854

11������origin�����滻��ֻ��Զ�̷�������һ�����ֶ��ѣ�

       git remote rename origin dev??

       git remote??

       ����dev??

       ��ȡgithub��Ŀ�ĵ�ַ

12����¡�ֿ⣺git clone

13��Զ�ֿ̲���������git remote rename oldName newName(�ⲽ�ɸĿɲ���)

14�����Դ�ֿ��ַΪԶ�ֿ̲⣺ git remote add

15���鿴�ļ��У� dir

����Ƚϣ�

16���ȽϹ��������ݴ����� git diff ?

17���Ƚ��ݴ����뱾�ذ汾�������һ��commit �����ݣ� git diff --cached

18���ȽϹ������뱾�ذ汾�������һ��commit������ ��git diff HEAD

19���Ƚ�����commit֮��Ĳ��죺 git diff

����������

20���鿴��֧�� git branch ?

21�������·�֧�� git branch ���½����Ҫ�л���֧��Ȼ��add��commit��push�������github������ʾ

22���������л���֧�� git checkout -b

23��ɾ�����ط�֧�� git branch -d

24��ɾ��Զ�̷�֧�� git push -d

25���л���֧�� git checkout

26��ɾ��ĳ���ļ��� git rm -r --cached target ɾ��target�ļ��к�commit��push��master

       master��װ��û��bug�Ĵ��룬dev��֧�Ǹ�masterһ���Ĵ��룬����������

27���ϲ���֧��git merge

28���ѱ���master��֧���͵�Զ�̵�master��֧�ϣ�

       git push origin master:master

       git push origin master:dev
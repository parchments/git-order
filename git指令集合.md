<h1>������Զ�̹��� </h1>

<h2>һ�������Ա����������ٶȿ죩</h2>
<p>       1�����ذ�װnode.js</p>
<p>https://nodejs.org/en/</p>

<p>2����װcnpm</p>
<p>       npm install -g cnpm --registry=https://registry.npm.taobao.org</p>

<p>3������Ƿ����óɹ� cnpm -v�����ְ汾����ɹ�</p>


<p>����SSH���ã���Զ�̹��������ã�</p>
<p>       SSH���ã�ssh-Keygen</p>
<p>       ������֮���ܵ�֪ssh���ļ�λ�ã����Ҹ���ssh�����key??</p>
<p>       Ȼ��Ѹ��Ƶ�keyճ����github-�ҵ�-setting-SSH and GPG keys-Add new��ȥ</p>

<h2>�������ػ������ã�</h2>
<p>       git config --global user.name 'xxx'</p>
<p>       git config --global user.email 123456789@qq.com</p>

�ġ�ָ��
<p>1����ʼ�����زֿ⣺git init</p>
<p>2�����Դ�ֿ⣺git remote add origin yourgithub���л���user-ssh��ַ��</p>
<p>3����Զ�ֿ̲����������������git pull origin </p>
<p>4������������鿴Զ�ֿ̲⣺git remote -v</p>
<p>5���鿴��ǰ�ļ���״̬�� git status</p>
<p>6���ύ���ݴ����� git add (��������ļ�����index.html���������ļ����á� . ����ķ�ʽ)</p>
<p>       �ݴ����ô������޸ĵ���ûд��Ͳ����ύ�����زֿ⣬�ύ�����زֿⶼ��һ���汾����һ��bug�ύ�����˺ϲ��ͻ�����⡣�ݴ����ᱻ���µĴ��븲��֮ǰ�Ĵ���</p>
<p>       �ŵ��ݴ�����</p>
<p>7���ύ�����زֿ⣺git commit -m ' �ύ��Ϣ�ļ�� '</p>
<p>8���ύ���ݵ�Զ�ֿ̲⣺ git push</p>
<p>9��������git checkout -- index.html</p>
<p>10���汾�Ż��ˣ�</p>
<p>       �鿴��־��ÿ���ύ��ʲô�� git log?</p>
<p>       ����commit �����b7dc85�ǰ汾�ţ����Խ��а汾�Ż���</p>

<p>       ����һ�������İ汾��--hard�����˵���һ�������İ汾</p>
<p>       git reset --hard HEAD~1??</p>
<p>       git reset --hard HEAD~2(���������汾)</p>

<p>       mixed���˵��ݴ������֮ǰ��״̬����add״̬</p>
<p>       soft֮��Ҫô�汾����Ҫô�ύ���˵�commit״̬</p>

<p>       ���˵�ָ���汾��git reflog</p>
<p>       git reset --hard b7dc854</p>

<p>11������origin�����滻��ֻ��Զ�̷�������һ�����ֶ��ѣ�</p>
<p>       git remote rename origin dev??</p>
<p>       git remote??</p>
<p>       ����dev??</p>
<p>       ��ȡgithub��Ŀ�ĵ�ַ</p>

<p>12����¡�ֿ⣺git clone</p>
<p>13��Զ�ֿ̲���������git remote rename oldName newName(�ⲽ�ɸĿɲ���)</p>
<p>14�����Դ�ֿ��ַΪԶ�ֿ̲⣺ git remote add</p>
<p>15���鿴�ļ��У� dir</p>

??
<p>����Ƚϣ�</p>
<p>16���ȽϹ��������ݴ����� git diff ?</p>
<p>17���Ƚ��ݴ����뱾�ذ汾�������һ��commit �����ݣ� git diff --cached</p>
<p>18���ȽϹ������뱾�ذ汾�������һ��commit������ ��git diff HEAD</p>
<p>19���Ƚ�����commit֮��Ĳ��죺 git diff</p>

<p>����������</p>
<p>20���鿴��֧�� git branch ?</p>
<p>21�������·�֧�� git branch ���½����Ҫ�л���֧��Ȼ��add��commit��push�������github������ʾ</p>
<p>22���������л���֧�� git checkout -b</p>
<p>23��ɾ�����ط�֧�� git branch -d</p>
<p>24��ɾ��Զ�̷�֧�� git push -d</p>
<p>25���л���֧�� git checkout</p>
<p>26��ɾ��ĳ���ļ��� git rm -r --cached target ?ɾ��target�ļ��к�commit��push��master</p>
<p>       master��װ��û��bug�Ĵ��룬dev��֧�Ǹ�masterһ���Ĵ��룬����������</p>
<p>27���ϲ���֧��git merge</p>
<p>28���ѱ���master��֧���͵�Զ�̵�master��֧�ϣ�</p>
<p>       git push origin master:master</p>
<p>       git push origin master:dev</p>
# naslite
# ����
- ����һ����Դ��������nas�������������http�������socks5���������̬web��������nasӦ�ý��̹���
- ����Ŀ��Դ���Ҹ��˵�����Windows Server 2022ϵͳ�������й���IP����Ҫ����ͥ���Ϳ���Ӱ�ã����Ӧ����FileBrowser,Jyellyfin,Gitea,SiYuan,Syncthing�ȣ��������Ӧ�þ�Ϊ��Դ��Ŀ���ǿ�Դ��Ŀ��Ӧ�û����ϲ����ǣ������ҵ�����Щ���Ӧ�û᲻����������δ��¶��©����������ͳһNAS��ڣ�������NASֻ��һ�����˿ڿ��ţ��������http/https����������к��Ӧ��ȫ�����ػ���ֻ��ͨ�����������ܷ��ʣ�����֧�ֶԺ��Ӧ�õĵ�¼�������أ���¼ʧ�ܴ������������IP��ֹ���ʣ�һ���̶��ϱ�����˺�����ı������ԣ������Щû����֤��Ҳû�жԵ�¼ʧ�ܽ��а�ȫ����ĺ��Ӧ�ã���һ���ı������ã�socks5�������������һЩ��������ķ���(��Զ������)�����SocksCap���������Ϳ���ʵ��NAS�ϵ�����Ӧ�ö�����ͨ�����������ܷ��ʣ�������ڵ���־��أ���������Ҳ�ܴ�������ԭ�������

# ����
- ��ȫ��Դ
- ��ˣ�C++23 boost asio coroutine
- ǰ�ˣ�vue3 + Element Plus
- Ŀǰ������Windowsϵͳ�µı����ʹ��

# ����ģ��
- http/https�������
- socks5�������
- ��̬http/https web������
- nasӦ�ý��̹���
- ֧��ͨ��web����Զ�̹���

# ����
## Windows
- ��װCMake, Visual Studio 2022, Node.js
### ������
- ����Ŀ��Ŀ¼������3rd,doc,frontend,CMakeLists.txt��Щ�ļ���Ŀ¼���Ǹ�Ŀ¼��
- ��cmd
- ִ���������
- cmake . -DCMAKE_BUILD_TYPE=Release -B build
- ��ɺ����buildĿ¼������Visual Studio 2022��.sln�����ļ���ʹ��Visual Studio 2022�������б��뼴��
- ��Ҫ�������Ŀ��(ֱ��F7���ɽ��������ȫ������Ҳ����)��naslite, prepose, windows-kill-library
- ����ֱ��ʹ������������б���
- cmake --build build --config Release
- ��ɺ����build/ReleaseĿ¼������exe��ִ�г������Ŀ�ļ�
### ����ǰ��
- ����Ŀ��Ŀ¼�е�frontend��Ŀ¼
- ��cmd
- ִ���������
- npm install
- npm run build
- ��ɺ���frontend/distĿ¼�����ɵ��ļ�����ǰ����ҳ�ļ�
## Linux
- ��װCMake, GCC, Node.js
- ������...

# ʹ��
## Windows
- ������NasLiteӦ�ã���������¼����ļ���
  - naslite.exe ���ĳ���
  - naslite.json �����ļ�����/naslite/naslite.json���ƹ������ɣ�
  - prepose.exe ֹͣ����ʱ���õ��ĸ�������
  - windows-kill-library.dll ֹͣ���̵ĺ��Ķ�̬��
- ��/naslite/naslite.json�����ļ����Ƶ�naslite.exe���ڵ�Ŀ¼��
- ��ǰ�����ǰ��ʱ�����ɵ�dist�ļ��и��ӵ�naslite.exe���ڵ�Ŀ¼��
- ����naslite.exe
- �������������http://127.0.0.1:8888�򿪺�̨����ҳ�棬Ĭ���˺�admin Ĭ������123456 ��¼֮��������������ü��ɣ�����ʹ����127.0.0.1�������̨����ֻ�ǳ�����ʾ���ã���Ҫ������ʹ��NasLite���й��ܣ�����Ҫ�������ſ��ԣ�
## Linux
- ������...

# ��ʾվ��
- ����NAS��[https://nav.nextvr.top:8888/](https://nav.nextvr.top:8888/)

# ���÷���
- ����-������DDNS SDK�� [https://api.aliyun.com/api/Alidns/2015-01-09/UpdateDomainRecord?tab=DEMO&lang=CSHARP](https://api.aliyun.com/api/Alidns/2015-01-09/UpdateDomainRecord?tab=DEMO&lang=CSHARP)
- SSL֤��(������)��win-acme

# webԶ�̹���(����Ӧ������Ļ���ֻ���)

![](./doc/index-pc.png)

![](./doc/http_reverse_proxy-pc.png)

![](./doc/service_process_mgr-phone.png)

![](./doc/frontend_http_server-phone.png)

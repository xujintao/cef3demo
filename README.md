# cef3demo
A demo for cef3

第一步：获得gyp源码
git clone https://chromium.googlesource.com/external/gyp

第二步：编译gyp源码得到gyp工具
1，下载安装python。
2，打开cmd，cd进入gyp目录，输入setup.py install

第三步：生成cefDemo的vs文件
1，进入cef目录
执行gyp.bat --depth=. -f msvs -G svs-version=2008
执行gyp --depth . -D component=shared_library -G msvs_version=2010 -l cef_paths.gypi -l cef_paths2.gypi

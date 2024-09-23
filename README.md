## 安装：
安装到系统库，可供Cmake直接找到  
1. 下载仓库：`git clone https://github.com/eclipse-iceoryx/iceoryx2.git && cd iceoryx2`
2. 安装RUST：`curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`
4. 安装依赖：`sudo ./internal/scripts/install_dependencies_ubuntu.sh`
5. 创建目录：`mkdir build && cd build/`
6. 构建与编译：`cmake .. && make`
7. 安装：`sudo make install`
8. 修改`ci_build_and_install_iceoryx_hoofs.sh`(位于iceoryx2/internal/scripts/)，将两处`-DCMAKE_INSTALL_PREFIX`后的目录改为`/usr/local`  
9. 执行`sudo ./ci_build_and_install_iceoryx_hoofs.sh`
---
试了一下Iox2已经支持多对多Topic了。  
---
安装不用看wiki直接cmake,make,install,再装hoofs和platform
---

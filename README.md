## 安装：
安装到系统库，可供Cmake直接找到  
1. 下载仓库：`git clone https://github.com/eclipse-iceoryx/iceoryx2.git`
2. 安装RUST：`curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`
3. 进入Iceoryx2目录
4. 安装依赖：`sudo ./internal/scripts/install_dependencies_ubuntu.sh`
5. Cmake构建：`cmake -S . -B target/ffi/build -DBUILD_EXAMPLES=ON`
6. 编译与安装：`sudo cmake --build target/ffi/build --target install`
7. 修改`ci_build_and_install_iceoryx_hoofs.sh`(位于iceoryx2/internal/scripts/)，将两处`-DCMAKE_INSTALL_PREFIX`后的目录改为`/usr/local`  
8. 执行`sudo ./ci_build_and_install_iceoryx_hoofs.sh`
---
试了一下Iox2已经支持多对多Topic了。  

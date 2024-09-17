# iceoryx2_install  
iceoryx2_install tutorial (with hoofs and platform)  
1. `curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`
2. `sudo ./internal/scripts/install_dependencies_ubuntu.sh`  
3. 进入iceoryx2主目录  
4. `cmake -S . -B target/ffi/build -DBUILD_EXAMPLES=ON`  
5. `sudo cmake --build target/ffi/build --target install`  
6. 更改ci_build_and_install_iceoryx_hoofs.sh（可以直接搜文件位置） ，将两个`-DCMAKE_INSTALL_PREFIX`后的位置改为`/usr/local`  
7. `sudo ./ci_build_and_install_iceoryx_hoofs.sh`
---
然后就可以独立编译这个官方例程了。  

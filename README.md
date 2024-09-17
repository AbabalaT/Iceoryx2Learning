# iceoryx2_install  
iceoryx2 install tutorial (with hoofs and platform)  
you can so install iceoryx2 to system library  
1. `git clone https://github.com/eclipse-iceoryx/iceoryx2.git`
2. `curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`
3. `sudo ./internal/scripts/install_dependencies_ubuntu.sh`
4. enter iceoryx2 directory
5. `cmake -S . -B target/ffi/build -DBUILD_EXAMPLES=ON`
6. `sudo cmake --build target/ffi/build --target install`
7. change ci_build_and_install_iceoryx_hoofs.sh(in iceoryx2/internal/scripts/), modify two paths after`-DCMAKE_INSTALL_PREFIX`to`/usr/local`  
8. `sudo ./ci_build_and_install_iceoryx_hoofs.sh`

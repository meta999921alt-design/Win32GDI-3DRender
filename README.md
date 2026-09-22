

## 요구 사항

- Windows 
- C++17 지원 컴파일러 (MSVC 또는 MinGW g++)
- CMake 3.10 이상

## 빌드

### CMake

```bash
mkdir build && cd build
cmake ..
cmake --build . --config Release
```

### MinGW

```bash
g++ -std=c++17 -O2 -mwindows -static -static-libgcc -static-libstdc++ -Iinclude src/*.cpp -o raytracer.exe -lgdi32 -luser32
```



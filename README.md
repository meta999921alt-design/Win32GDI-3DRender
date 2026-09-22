

## 요구 사항

- Windows 
- C++17 지원 컴파일러 (MSVC 또는 MinGW g++)
- CMake 3.10 이상 (선택 — 없어도 g++로 직접 빌드 가능)

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



## 실행

- **WASD**: 이동
- **마우스 우클릭 드래그**: 시선 회전
- **ESC** 또는 창 닫기: 종료

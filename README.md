# boost 라이브러리 설치 방법

### mac에서 설치 방법

> **CLI**
> 

```bash
brew install boost
```

> **CMAKELISTS**
> 

```cpp
#Boost 라이브러리 설치 확인
find_package(Boost)

if(Boost_FOUND)
    # include 패스 설정
    include_directories(${Boost_INCLUDE_DIRS})
endif()
```
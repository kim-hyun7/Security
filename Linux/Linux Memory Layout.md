# Code Segment (Text Segment)

    실행 가능한 기계 코드가 위치하는 영역

- 권한: 읽기 및 실행

```c
    int main() { return 31337; }
```

ex: 리턴값 31337 → 기계코드 554889e5b8697a00005dc3 변환 후 코드 세그먼트에 위치.

# Data Segment

    파일 시점에 값이 정해진 전역 변수 및 전역 상수

- ### Data Segment
  쓰기가 가능한 세그먼트로, 실행되면서 값이 변할 수 있는 데이터들이 위치한다.
- ### Rodata Segment (Read Only Data)
  쓰기가 불가능한 세그먼트로, 값이 변하면 안되는 데이터들이 위치한다.

```c
int data_num = 31337;                       // data
char data_rwstr[] = "writable_data";        // data
const char data_rostr[] = "readonly_data";  // rodata
char *str_ptr = "readonly";  // str_ptr은 data, 문자열은 rodata
int main() { ... }
```

# BSS Segment (Block Started By Symbol Semgent)

    컴파일 시점에 값이 정해지지 않은 전역 변수

개발자가 선언만 하고 초기화되지 않는 전역 변수 등이 포함된다.

```c
int bss_data; // 개발자가 초기화 하지 않았으므로 값은 0으로 초기화된다.

int main() {
  printf("%d\n", bss_data);  // 0
  return 0;
}
```

# Stack Segment

    프로세스의 스택이 위치하는 영역. 함수의 인자나 지역 변수와 같은 임시 변수들이 실행중에 여기에 저장된다.

```c
void func() {
  int choice = 0;
  scanf("%d", &choice);
  if (choice)
    call_true();
  else
    call_false();
  return 0;
}
```

지역 변수 choice는 스택에 저장된다.

# Heap Segment

    실행중에 동적으로 할당될 수 있으며, 리눅스에서는 스택 세그먼트와 반대 방향으로 자란다.

- 동적 할당

  프로그램 실행 단계에서 결정되는 크기에 따라 메모리를 할당해주는 방식이다.

  상황에 따라 필요한 만큼의 메모리를 할당받을 수 있다.

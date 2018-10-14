# cpp-conventions
C++ conventions I have adopted.

```
// common.h
#pragma once

#include <stdint.h>
//#include <stdbool.h> -- C only

typedef uint8_t u8;
typedef uint16_t u16;
typedef uint32_t u32;
typedef uint64_t u64;

typedef int8_t i8;
typedef int16_t i16;
typedef int32_t i32;
typedef int64_t i64;

typedef float f32;
typedef double f64;

#define internal static // for functions without header pairings
#define global_variable static // for variables within file scope
#define local_persist static // for variables within function scope
```

```
struct type_name {
    int data;
};
```
 
```
void my_function_name(int arguments_n_such) {
    type_name stuff;
    stuff.data = arguments_n_such;
}
```

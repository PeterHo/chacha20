# chacha20

网上搜集并修改过的chacha20序列加密算法代码

可以修改chacha20.h中的sigma的值来改变初始化条件

使用方法

```
#include "chacha20.h"

unsigned char in[100]; // 输入
unsigned int inLen = sizof(in); // 输入大小
unsigned char out[100]; // 输出
unsigned char key[32]; // 密钥
unsigned char nonce[12]; // 临时密钥
ChaCha20XOR(out, in, inLen, key, nonce, 0);
```

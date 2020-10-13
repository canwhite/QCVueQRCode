# QCVueQRCode
生成二维码的组件
---
注意Lib文件夹要和vue-qrcode放在一起，因为vue-qrcode.js
里会引入Lib中的工具

#### 1.引入
```
//注意自己放的相对位置
import QrcodeVue from '../../js/vue-qrcode';

...

components: {
    QrcodeVue
},

```
#### 2.在具体使用的时候
```

<qrcode-vue :value="value" :size="size" level="H"></qrcode-vue>

...

data() {
    return {

        value:"hello world",//二维码分享的内容
        size: 150,

    };
},



```
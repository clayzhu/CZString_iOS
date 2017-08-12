# CZString_iOS
对字符串进行操作的一些方法的封装，用于判断字符串是否为空、切割字符串、获取字符串中中英文字符等。

## 介绍

在解析网络请求的数据时，服务器可能会返回 `(null)`、`@""`、`nil` 等，这些数据在客户端这边显示上都应当解释为无数据。因此需要一些判断和格式化，来判断字符串是否为空，并返回正确的空串。

另外，纯数字的字符串在传递过程中会被 Objective-C 自动转换为 NSNumber 类型，此时如果使用 `isEqualToString:` 或赋值给 `label.text` 等一些字符串操作，程序会 crash。


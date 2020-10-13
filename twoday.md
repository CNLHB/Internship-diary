**20.10.13**

**上午**

+ JS基本内置对象概述，分类

- 

- String

  - 字符串书写形式

    + 单引号，双引号, 显示示换行表示  'a \n b'     代码换行，显示不换行 'a \ b', 字符串模板
    + 转义
      + 表示unicode
        + \xFFFF
        + \uXXXX
      + 表示emoji
        + \u{xxxx}

  - 方法

    + 搜索

      + 返回指定位置字符

        + charAt 返回字符
        + charCodeAt 返回unicode字符
        + codePointAt  返回uft-16编码

      + 判断字符串是否包含子串

        + 判断一个字符串里是否包含其他字符串。str1.includes(str2)
        + 判断一个字符串的是否以给定字符串结尾，结果返回布尔值。 String.prototype.endsWith()
        + 从字符串对象中返回首个被发现的给定值的索引值，如果没有找到则返回-1。String.prototype.indexOf()
        + 从字符串对象中返回最后一个被发现的给定值的索引值，如果没有找到则返回-1。lastIndexOf()

      + String.prototype.match()

        使用正则表达式与字符串相比较。

      + String.prototype.search()

        对正则表达式和指定字符串进行匹配搜索，返回第一个出现的匹配项的下标。

    + 转换

      + 字符串拼接返回新字符串 str.concat(str2)

      + slice  摘取一个字符串区域，返回一个新的字符串     长度

      + String.prototype.substr()

        通过指定字符数返回在指定位置开始的字符串中的字符。  长度

      + String.prototype.substring()

        返回在字符串中指定两个下标之间的字符。 截取下标

    + 替换

      + replace()

    + 修饰

      + 格式化
      + trim()
      + trimLeft
      + trimRight

    + 系列化

      + 系列化成数组
        + split('')

-  Number
   -  number书写形式
      + 字面量10进制表示
      + 16进制表示
      + 安全整数
      + 精度判断
      + Number对象常量
      + 方法
        + 判断是否为某个特殊值
          + 确定传递的值是否是 NaN。  Number.isNaN
          + 确定传递的值类型及本身是否是有限数。Number.isFinite
        + 系列化
          + Number.parseInt
          + Number.parseFloat
          + .toFixed()

​    **下午**

- Object 重点
  - 创建对象
    - 字面量   let obj = {}
    - new关键字  let obj = new Object() 
    - Object.create(原型链指向) 使用指定的原型对象和属性创建一个新对象。
    - Object.assign  方法用于将所有可枚举属性的值从一个或多个源对象复制到目标对象。它将返回目标对象。
  - 实例方法
    - toString
    - valueOf
    - hasOwnProperty  判断是否为自身的属性
  - 静态方法
    - 添加属性和指定配置
      - 添加一个
        - Object.definePerproty
      - 添加多个
        - Object.definePerproties
    - 获取可枚举对象的key、value
      - Object.key
      - Object.value
      - Object.entries
    - 获取对象属性或属性配置
      - 返回对象指定的属性配置。Object.getOwnPropertyDescriptor()
      - 返回一个数组，它包含了指定对象所有的可枚举或不可枚举的属性名。Object.getOwnPropertyNames()
      - 返回一个数组，它包含了指定对象自身所有的符号属性。Object.getOwnPropertySymbols()
      - 返回指定对象的原型对象。Object.getPrototypeOf
    - 冻结对象
      - 冻结对象：其他代码不能删除或更改任何属性。Object.freeze()
      - 封闭一个对象，阻止添加新属性并将所有现有属性标记为不可配置。当前属性的值只要原来是可写的就可以改变。Object.seal()
- 分享几个小题目
- 提问解答



今日记录



重新梳理Number、String、Object的属性和方法

并对属性和方法归类，以便于记忆
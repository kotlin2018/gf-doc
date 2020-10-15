[TOC]

# 错误提示

`gvalid`默认的错误提示是英文的，并且错误提示使用了`i18n`特性，也就是说我们可以通过配置`i18n`文件即可替换默认的错误提示。`i18n`国际化功能请参考【[gi18n (国际化处理)](i18n/gi18n/index.md)】章节。

## 默认`i18n`错误提示

默认的英文国际化语言配置文件参考：https://github.com/gogf/gf/tree/master/util/gvalid/i18n/en
```toml
"gf.gvalid.rule.required"             = "The :attribute field is required"
"gf.gvalid.rule.required-if"          = "The :attribute field is required"
"gf.gvalid.rule.required-unless"      = "The :attribute field is required"
"gf.gvalid.rule.required-with"        = "The :attribute field is required"
"gf.gvalid.rule.required-with-all"    = "The :attribute field is required"
"gf.gvalid.rule.required-without"     = "The :attribute field is required"
"gf.gvalid.rule.required-without-all" = "The :attribute field is required"
"gf.gvalid.rule.date"                 = "The :attribute value is not a valid date"
"gf.gvalid.rule.date-format"          = "The :attribute value does not match the format :format"
"gf.gvalid.rule.email"                = "The :attribute value must be a valid email address"
"gf.gvalid.rule.phone"                = "The :attribute value must be a valid phone number"
"gf.gvalid.rule.telephone"            = "The :attribute value must be a valid telephone number"
"gf.gvalid.rule.passport"             = "The :attribute value is not a valid passport format"
"gf.gvalid.rule.password"             = "The :attribute value is not a valid passport format"
"gf.gvalid.rule.password2"            = "The :attribute value is not a valid passport format"
"gf.gvalid.rule.password3"            = "The :attribute value is not a valid passport format"
"gf.gvalid.rule.postcode"             = "The :attribute value is not a valid passport format"
"gf.gvalid.rule.resident-id"          = "The :attribute value is not a valid resident id number"
"gf.gvalid.rule.bank-card"            = "The :attribute value must be a valid bank card number"
"gf.gvalid.rule.qq"                   = "The :attribute value must be a valid QQ number"
"gf.gvalid.rule.ip"                   = "The :attribute value must be a valid IP address"
"gf.gvalid.rule.ipv4"                 = "The :attribute value must be a valid IPv4 address"
"gf.gvalid.rule.ipv6"                 = "The :attribute value must be a valid IPv6 address"
"gf.gvalid.rule.mac"                  = "The :attribute value must be a valid MAC address"
"gf.gvalid.rule.url"                  = "The :attribute value must be a valid URL address"
"gf.gvalid.rule.domain"               = "The :attribute value must be a valid domain format"
"gf.gvalid.rule.length"               = "The :attribute value length must be between :min and :max"
"gf.gvalid.rule.min-length"           = "The :attribute value length must be equal or greater than :min"
"gf.gvalid.rule.max-length"           = "The :attribute value length must be equal or lesser than :max"
"gf.gvalid.rule.between"              = "The :attribute value must be between :min and :max"
"gf.gvalid.rule.min"                  = "The :attribute value must be equal or greater than :min"
"gf.gvalid.rule.max"                  = "The :attribute value must be equal or lesser than :max"
"gf.gvalid.rule.json"                 = "The :attribute value must be a valid JSON string"
"gf.gvalid.rule.xml"                  = "The :attribute value must be a valid XML string"
"gf.gvalid.rule.array"                = "The :attribute value must be an array"
"gf.gvalid.rule.integer"              = "The :attribute value must be an integer"
"gf.gvalid.rule.float"                = "The :attribute value must be a float"
"gf.gvalid.rule.boolean"              = "The :attribute value field must be true or false"
"gf.gvalid.rule.same"                 = "The :attribute value must be the same as field :field"
"gf.gvalid.rule.different"            = "The :attribute value must be different from field :field"
"gf.gvalid.rule.in"                   = "The :attribute value is not in acceptable range"
"gf.gvalid.rule.not-in"               = "The :attribute value is not in acceptable range"
"gf.gvalid.rule.regex"                = "The :attribute value is invalid"
"gf.gvalid.rule.__default__"          = "The :attribute value is invalid"
```

## 中文错误提示

我们提供了建议的中文`i18n`国际化语言配置文件：https://github.com/gogf/gf/tree/master/util/gvalid/i18n/cn
```toml
"gf.gvalid.rule.required"             = ":attribute 字段不能为空"
"gf.gvalid.rule.required-if"          = ":attribute 字段不能为空"
"gf.gvalid.rule.required-unless"      = ":attribute 字段不能为空"
"gf.gvalid.rule.required-with"        = ":attribute 字段不能为空"
"gf.gvalid.rule.required-with-all"    = ":attribute 字段不能为空"
"gf.gvalid.rule.required-without"     = ":attribute 字段不能为空"
"gf.gvalid.rule.required-without-all" = ":attribute 字段不能为空"
"gf.gvalid.rule.date"                 = ":attribute 日期格式不正确"
"gf.gvalid.rule.date-format"          = ":attribute 日期格式不满足:format"
"gf.gvalid.rule.email"                = ":attribute 邮箱地址格式不正确"
"gf.gvalid.rule.phone"                = ":attribute 手机号码格式不正确"
"gf.gvalid.rule.telephone"            = ":attribute 电话号码格式不正确"
"gf.gvalid.rule.passport"             = ":attribute 账号格式不合法，必需以字母开头，只能包含字母、数字和下划线，长度在6~18之间"
"gf.gvalid.rule.password"             = ":attribute 密码格式不合法，密码格式为任意6-18位的可见字符"
"gf.gvalid.rule.password2"            = ":attribute 密码格式不合法，密码格式为任意6-18位的可见字符，必须包含大小写字母和数字"
"gf.gvalid.rule.password3"            = ":attribute 密码格式不合法，密码格式为任意6-18位的可见字符，必须包含大小写字母、数字和特殊字符"
"gf.gvalid.rule.postcode"             = ":attribute 邮政编码不正确"
"gf.gvalid.rule.resident-id"          = ":attribute 身份证号码格式不正确"
"gf.gvalid.rule.bank-card"            = ":attribute 银行卡号格式不正确"
"gf.gvalid.rule.qq"                   = ":attribute QQ号码格式不正确"
"gf.gvalid.rule.ip"                   = ":attribute IP地址格式不正确"
"gf.gvalid.rule.ipv4"                 = ":attribute IPv4地址格式不正确"
"gf.gvalid.rule.ipv6"                 = ":attribute IPv6地址格式不正确"
"gf.gvalid.rule.mac"                  = ":attribute MAC地址格式不正确"
"gf.gvalid.rule.url"                  = ":attribute URL地址格式不正确"
"gf.gvalid.rule.domain"               = ":attribute 域名格式不正确"
"gf.gvalid.rule.length"               = ":attribute 字段长度为:min到:max个字符"
"gf.gvalid.rule.min-length"           = ":attribute 字段最小长度为:min"
"gf.gvalid.rule.max-length"           = ":attribute 字段最大长度为:max"
"gf.gvalid.rule.between"              = ":attribute 字段大小为:min到:max"
"gf.gvalid.rule.min"                  = ":attribute 字段最小值为:min"
"gf.gvalid.rule.max"                  = ":attribute 字段最大值为:max"
"gf.gvalid.rule.json"                 = ":attribute 字段应当为JSON格式"
"gf.gvalid.rule.xml"                  = ":attribute 字段应当为XML格式"
"gf.gvalid.rule.array"                = ":attribute 字段应当为数组"
"gf.gvalid.rule.integer"              = ":attribute 字段应当为整数"
"gf.gvalid.rule.float"                = ":attribute 字段应当为浮点数"
"gf.gvalid.rule.boolean"              = ":attribute 字段应当为布尔值"
"gf.gvalid.rule.same"                 = ":attribute 字段值必须和:field相同"
"gf.gvalid.rule.different"            = ":attribute 字段值不能与:field相同"
"gf.gvalid.rule.in"                   = ":attribute 字段值不合法"
"gf.gvalid.rule.not-in"               = ":attribute 字段值不合法"
"gf.gvalid.rule.regex"                = ":attribute 字段值不合法"
"gf.gvalid.rule.__default__"          = ":attribute 字段值不合法"
```


## `__default__`错误提示

当在`i18n`中找不到对应规则的错误提示时，将会使用`__default__`配置的错误提示信息。往往使用在自定义规则中。






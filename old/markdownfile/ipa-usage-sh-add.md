
#####shenzhen 是命令行编译发布ipa的工具。用起来很方便，是用ruby写的
github地址在 https://github.com/nomad/shenzhen

```
ipa build -w App.xcworkspace -s Scheme -m "XYZ.mobileprovision" -i "YYY" --xcargs 'CODE_SIGN_ENTITLEMENTS="Entitlements.plist" CODE_SIGN_IDENTITY="iPhone Distribution: XXX (YYY)"'

-w App.xcworkspace
-s Scheme
-m "XYZ.mobileprovision"
-i "YYY"
--xcargs 'CODE_SIGN_ENTITLEMENTS="Entitlements.plist" CODE_SIGN_IDENTITY="iPhone Distribution: XXX (YYY)"'
-c Release  or Debug 
```
#####显示应用签名信息
```
codesign -vv -d test.app

Executable=/Users/me/Desktop/test/Payload/test.app/test
Identifier=com.testapp.testapp
Format=bundle with Mach-O universal (armv7 armv7s)
CodeDirectory v=20100 size=36441 flags=0x0(none) hashes=1818+5 location=embedded
Signature size=3483
Authority=Apple iPhone OS Application Signing
Authority=Apple iPhone Certification Authority
Authority=Apple Root CA
Info.plist entries=35
TeamIdentifier=KB7T8S4E4U
Sealed Resources version=2 rules=5 files=1240
Internal requirements count=1 size=100
```

```
codesign --display -r- Payload/test.app 
Executable=/Users/me/Desktop/test/Payload/test.app/test
designated => anchor apple generic and certificate leaf[field.1.2.840.113635.100.6.1.3] /* exists */ and identifier "com.test.test"
```
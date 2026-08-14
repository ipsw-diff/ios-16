## AppPredictionInternal

> `/System/Library/PrivateFrameworks/AppPredictionInternal.framework/AppPredictionInternal`

```diff

-508.33.0.0.0
-  __TEXT.__text: 0x3e21c8
+508.33.1.0.0
+  __TEXT.__text: 0x3e2304
   __TEXT.__stubs: 0x15e4
-  __TEXT.__objc_methlist: 0x38488
+  __TEXT.__objc_methlist: 0x38490
   __TEXT.__const: 0x349e
   __TEXT.__cstring: 0x4f2fb
-  __TEXT.__oslogstring: 0x36d5b
+  __TEXT.__oslogstring: 0x36dc7
   __TEXT.__gcc_except_tab: 0xc894
   __TEXT.__dlopen_cstrs: 0x27a
   __TEXT.__ustring: 0x4
-  __TEXT.__unwind_info: 0xcd00
+  __TEXT.__unwind_info: 0xcd04
   __TEXT.__eh_frame: 0x108
   __TEXT.__objc_classname: 0x8ba1
-  __TEXT.__objc_methname: 0xaae8b
+  __TEXT.__objc_methname: 0xaaeb1
   __TEXT.__objc_methtype: 0x19b40
-  __TEXT.__objc_stubs: 0x4cbe0
-  __DATA_CONST.__got: 0x16c0
+  __TEXT.__objc_stubs: 0x4cc00
+  __DATA_CONST.__got: 0x16c8
   __DATA_CONST.__const: 0x110f0
   __DATA_CONST.__cfstring: 0x37fc0
   __DATA_CONST.__objc_classlist: 0x1e00

   __DATA_CONST.__objc_protolist: 0x428
   __DATA_CONST.__objc_imageinfo: 0x8
   __DATA_CONST.__objc_const: 0x851e0
-  __DATA_CONST.__objc_selrefs: 0x1bf18
+  __DATA_CONST.__objc_selrefs: 0x1bf20
   __DATA_CONST.__objc_intobj: 0x3558
   __DATA_CONST.__objc_arraydata: 0x1400
   __DATA_CONST.__objc_arrayobj: 0x11b8

   - /usr/lib/libcompression.dylib
   - /usr/lib/libobjc.A.dylib
   - /usr/lib/libsqlite3.dylib
-  Functions: 24379
-  Symbols:   46124
-  CStrings:  32810
+  Functions: 24380
+  Symbols:   46128
+  CStrings:  32812
 
Symbols:
+ -[ATXNotificationAndSuggestionDatabase _purgeNotificationBiomeStreamsIfNeeded]
+ GCC_except_table161
+ GCC_except_table166
+ __kATXBiomeNotificationPurgeCompleteKey
+ _objc_msgSend$_purgeNotificationBiomeStreamsIfNeeded
- GCC_except_table160
Functions:
~ -[ATXNotificationAndSuggestionDatabase init] : 116 -> 124
+ -[ATXNotificationAndSuggestionDatabase _purgeNotificationBiomeStreamsIfNeeded]
~ -[ATXNotificationsLoggingServer logNotificationEvent:notification:reason:] : 912 -> 964
CStrings:
+ "ATXNotificationAndSuggestionDatabase: Purging private notification streams to remove persisted text content"
+ "_purgeNotificationBiomeStreamsIfNeeded"
```

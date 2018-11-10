# HLFaker
HLFaker - Android AutoLead

--HLFaker Controller version 2.8.3--
- Add some InApp Tab functions.
- Extrack platform-tools.zip to C:\platform-tools\adb.exe. Add Enviroment Variables: Path: C:\platform-tools\
- Start ADB: adb start-server in command line.

--> Install HLFaker & HLBrowser:
+ Root device with SuperSU or Magisk.
+ Install Xposed, Xposed Framework for SuperSU or Magisk.
+ Install Busybox for SuperSU or Magisk.
+ Install HLBrowser APK: Don't need OPEN
+ Install HLFaker APK: OPEN and Allow root permission
+ Open Xposed -> Module: Tick HLFaker 3.1.1 module
+ Reboot device. Wait HLFaker service launch on notication center.
+ Open HLFaker Controller on PC and connect to device IP with same WiFi. Dub click on serial to copy and send me.
<img src="https://i.imgur.com/jHvAn7G.png">

CÚ PHÁP VIÊT SCRIPT CHO AUTO

ah:0 or ah:1
- Disable/Enable AndHook

cmd:command
- vd: pm uninstall com.igg.android.lordsmobile
- Chạy một lệnh shell trên thiết bị.

openapp:package
- vd: openapp:com.igg.android.lordsmobile

closeapp:package
- vd: closeapp:com.igg.android.lordsmobile

copyfile:fileNguon|fileDich
- vd: copyfile:/sdcard/test.txt|/sdcard/test/abc.txt

randomtouch:package,number
- vd: randomtouch:com.igg.android.lordsmobile,500
- Mở package com.igg.android.lordsmobile và random 500 lệnh touch

touch:X,Y
- Click vào tọa độ X,Y Ví dụ: touch:100,200

swipe:X1,Y1,X2,Y2
- Swipe(vuốt) từ tọa độ XY1 đến XY2 Ví dụ: swipe:100,200,300,400

text:yourtext/random,min,max
- Nhập vào một đoạn text hoặc tạo ngẫu nhiêu một đoạn text 
- Ví dụ: text:my name hoặc text:random,2,8

email:random/random@domain
- Tạo ngẫu nhiên một địa chỉ email Ví dụ: email:random hoặc email:random@gmail.com

phone:xxx-length
- Tạo ngẫu nhiên một số điện thoại theo đầu số Ví dụ: phone:096-10

password:symbol,min,max
- Tạo ngẫu nhiên mật khẩu theo ký tự đã cho và độ dài mật khẩu
- Ví dụ: password:abcdexzy124,6,8

firstname:random
- Tạo ngẫu nhiên First Name

lastname:random
- Tạo ngẫu nhiên Last Name

fullname:random
- Tạo ngẫu nhiên một Tên đầy đủ

username:min,max
- Tạo ngẫu nhiên tên tài khoản Ví dụ: username:6,10

delay:s
- Chờ s giây: Ví dụ: delay:20

paste:text
- Nhập lại password, email đã nhập trước đó Ví dụ: paste:text

layout:
- Đọc thông tin giao diện(chữ) ở màn hình điện thoại lúc gọi lệnh
- Ví dụ: layout:

clicktext:text|true/false
- Click vào text có trên màn hình điện thoại. Giá trị “true” click vào text có trên màn hình mà không yêu cầu phải đúng 100%. Giá trị “false” phải click đúng vào text yêu cầu(Khớp 100% và phân biệt hoa thường).

keyevent:KEYCODE
- Gửi một đoạn KEYCODE của Android đến điện thoại Ví dụ: keyevent:KEYCODE_BACK

Danh sách KEY Event của Android. Có thể dùng số hoặc chữ
0 -->  "KEYCODE_UNKNOWN" 
1 -->  "KEYCODE_MENU" 
2 -->  "KEYCODE_SOFT_RIGHT" 
3 -->  "KEYCODE_HOME" 
4 -->  "KEYCODE_BACK" 
5 -->  "KEYCODE_CALL" 
6 -->  "KEYCODE_ENDCALL" 
7 -->  "KEYCODE_0" 
8 -->  "KEYCODE_1" 
9 -->  "KEYCODE_2" 
10 -->  "KEYCODE_3" 
11 -->  "KEYCODE_4" 
12 -->  "KEYCODE_5" 
13 -->  "KEYCODE_6" 
14 -->  "KEYCODE_7" 
15 -->  "KEYCODE_8" 
16 -->  "KEYCODE_9" 
17 -->  "KEYCODE_STAR" 
18 -->  "KEYCODE_POUND" 
19 -->  "KEYCODE_DPAD_UP" 
20 -->  "KEYCODE_DPAD_DOWN" 
21 -->  "KEYCODE_DPAD_LEFT" 
22 -->  "KEYCODE_DPAD_RIGHT" 
23 -->  "KEYCODE_DPAD_CENTER" 
24 -->  "KEYCODE_VOLUME_UP" 
25 -->  "KEYCODE_VOLUME_DOWN" 
26 -->  "KEYCODE_POWER" 
27 -->  "KEYCODE_CAMERA" 
28 -->  "KEYCODE_CLEAR" 
29 -->  "KEYCODE_A" 
30 -->  "KEYCODE_B" 
31 -->  "KEYCODE_C" 
32 -->  "KEYCODE_D" 
33 -->  "KEYCODE_E" 
34 -->  "KEYCODE_F" 
35 -->  "KEYCODE_G" 
36 -->  "KEYCODE_H" 
37 -->  "KEYCODE_I" 
38 -->  "KEYCODE_J" 
39 -->  "KEYCODE_K" 
40 -->  "KEYCODE_L" 
41 -->  "KEYCODE_M" 
42 -->  "KEYCODE_N" 
43 -->  "KEYCODE_O" 
44 -->  "KEYCODE_P" 
45 -->  "KEYCODE_Q" 
46 -->  "KEYCODE_R" 
47 -->  "KEYCODE_S" 
48 -->  "KEYCODE_T" 
49 -->  "KEYCODE_U" 
50 -->  "KEYCODE_V" 
51 -->  "KEYCODE_W" 
52 -->  "KEYCODE_X" 
53 -->  "KEYCODE_Y" 
54 -->  "KEYCODE_Z" 
55 -->  "KEYCODE_COMMA" 
56 -->  "KEYCODE_PERIOD" 
57 -->  "KEYCODE_ALT_LEFT" 
58 -->  "KEYCODE_ALT_RIGHT" 
59 -->  "KEYCODE_SHIFT_LEFT" 
60 -->  "KEYCODE_SHIFT_RIGHT" 
61 -->  "KEYCODE_TAB" 
62 -->  "KEYCODE_SPACE" 
63 -->  "KEYCODE_SYM" 
64 -->  "KEYCODE_EXPLORER" 
65 -->  "KEYCODE_ENVELOPE" 
66 -->  "KEYCODE_ENTER" 
67 -->  "KEYCODE_DEL" 
68 -->  "KEYCODE_GRAVE" 
69 -->  "KEYCODE_MINUS" 
70 -->  "KEYCODE_EQUALS" 
71 -->  "KEYCODE_LEFT_BRACKET" 
72 -->  "KEYCODE_RIGHT_BRACKET" 
73 -->  "KEYCODE_BACKSLASH" 
74 -->  "KEYCODE_SEMICOLON" 
75 -->  "KEYCODE_APOSTROPHE" 
76 -->  "KEYCODE_SLASH" 
77 -->  "KEYCODE_AT" 
78 -->  "KEYCODE_NUM" 
79 -->  "KEYCODE_HEADSETHOOK" 
80 -->  "KEYCODE_FOCUS" 
81 -->  "KEYCODE_PLUS" 
82 -->  "KEYCODE_MENU" 
83 -->  "KEYCODE_NOTIFICATION" 
84 -->  "KEYCODE_SEARCH" 
85 -->  "TAG_LAST_KEYCODE"

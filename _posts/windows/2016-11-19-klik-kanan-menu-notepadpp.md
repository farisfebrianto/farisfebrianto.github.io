---
layout: post
title:  "Klik Kanan Menu Notepad++"
categories: windows
---

Notepad++ yaitu software untuk mengedit berbagai jenis plain text dan mempunyai banyak keunggulan seperti syntax hightlighting, auto completetion, ringan, dan tentunya open source. Jika kalian menginstal versi installer, ketika kalian klik kanan suatu file maka akan muncul opsi Edit with Notepad++.

<!--more-->

Tutorial

Berbeda lagi dengan versi portablenya yang tidak mengintegrasikan pilihan ini karena tidak mengubah registry windows sama sekali. Solusinya kalian tulis kode berikut dan simpan dengan ekstensi .reg kemudian kalian eksekusi. Ganti file path notepad++ sesuai kalian taruh notepad++ versi portable kalian, kalau saya menaruhnya di folder D:/System/Program Files/Notepad++

```
Windows Registry Editor Version 5.00

[HKEY_CLASSES_ROOT\*\shellex\ContextMenuHandlers\ANotepad++] @="{00F3C2EC-A6EE-11DE-A03A-EF8F55D89593}"
[HKEY_CLASSES_ROOT\CLSID\{00F3C2EC-A6EE-11DE-A03A-EF8F55D89593}] @="ANotepad++"
[HKEY_CLASSES_ROOT\CLSID\{00F3C2EC-A6EE-11DE-A03A-EF8F55D89593}\InprocServer32] @="D:\\System\\Program Files\\Notepad++\\NppShell_05.dll" "ThreadingModel"="Apartment"
[HKEY_CLASSES_ROOT\CLSID\{00F3C2EC-A6EE-11DE-A03A-EF8F55D89593}\Settings] "Title"="Edit with &Notepad++" "Path"="D:\\System\\Program Files\\Notepad++\\notepad++.exe" "Custom"="" "ShowIcon"=dword:00000001 "Dynamic"=dword:00000001 "Maxtext"=dword:00000019

[HKEY_LOCAL_MACHINE\SOFTWARE\Classes\*\shellex\ContextMenuHandlers\ANotepad++] @="{00F3C2EC-A6EE-11DE-A03A-EF8F55D89593}"
[HKEY_LOCAL_MACHINE\SOFTWARE\Classes\CLSID\{00F3C2EC-A6EE-11DE-A03A-EF8F55D89593}] @="ANotepad++"
[HKEY_LOCAL_MACHINE\SOFTWARE\Classes\CLSID\{00F3C2EC-A6EE-11DE-A03A-EF8F55D89593}\InprocServer32] @="D:\\System\\Program Files\\Notepad++\\NppShell_05.dll" "ThreadingModel"="Apartment"
[HKEY_LOCAL_MACHINE\SOFTWARE\Classes\CLSID\{00F3C2EC-A6EE-11DE-A03A-EF8F55D89593}\Settings] "Title"="Edit with &Notepad++" "Path"="D:\\System\\Program Files\\Notepad++\\notepad++.exe" "Custom"="" "ShowIcon"=dword:00000001 "Dynamic"=dword:00000001 "Maxtext"=dword:00000019
[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\App Paths\notepad++.exe] @="D:\\System\\Program Files\\Notepad++\\notepad++.exe"
```

Setelah selesai menambahkan registry, silahkan coba klik kanan pada file apa saja. Jika tidak muncul `Open with Notepad++` coba periksa lagi dengan teliti :(

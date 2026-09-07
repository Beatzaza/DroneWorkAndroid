โปรเจกต์ Android: โดรนพ่นยา - ตารางงาน
ต้นฉบับ: drone_app_exact_style_v6_tomorrow.zip

วิธีสร้าง APK บน Windows ด้วย Android Studio
1) ติดตั้ง Android Studio
2) แตก ZIP นี้
3) เปิดโฟลเดอร์ DroneWorkAndroid ใน Android Studio
4) รอ Gradle Sync ให้เสร็จ
5) เมนู Build > Build App Bundle(s) / APK(s) > Build APK(s)
6) APK จะอยู่ที่ app/build/outputs/apk/debug/app-debug.apk

ข้อมูลตารางงานของเว็บแอปจะเก็บใน WebView local storage ของแอปบนเครื่อง Android
ดังนั้นข้อมูลจะอยู่ในมือถือเครื่องนั้นจนกว่าจะล้างข้อมูลแอป/ถอนการติดตั้ง

ทางเลือกไม่ต้องติดตั้ง Android Studio:
โปรเจกต์มี .github/workflows/build-apk.yml
อัปโหลดโปรเจกต์ขึ้น GitHub แล้วเปิด Actions > Build Android APK > Run workflow
เมื่อเสร็จ ดาวน์โหลด artifact ชื่อ DroneWork-APK จะมี app-debug.apk

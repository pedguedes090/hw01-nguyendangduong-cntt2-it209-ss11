# Bài 1 — GitHub Actions chạy JUnit với Gradle

**Sinh viên:** Nguyễn Đăng Dương  
**Lớp:** CNTT2  
**Môn học:** IT209 — Session 11

Workflow `.github/workflows/ci.yml` tự chạy khi có push lên `main`, cài Temurin JDK 17, cấp quyền thực thi cho Gradle Wrapper và chạy `./gradlew test`. Dự án Spring Boot có bài kiểm thử nạp application context để job kiểm tra được thực tế.

## Chạy cục bộ

```bash
./gradlew test
```

Trên Windows có thể chạy `gradlew.bat test`.

## Kiểm tra kết quả

Mở tab **Actions** của repository và xác nhận job **Run Unit Tests** hoàn tất thành công.


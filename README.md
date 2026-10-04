# 🕌 Masjid Nurul Amal — Android WebView

Aplikasi TV Masjid berbasis WebView untuk **Masjid Nurul Amal, Rajabasa, Bandar Lampung**.

## Fitur
- Tampilan TV masjid landscape/fullscreen
- Video masjid bergantian
- Jadwal sholat
- Countdown sholat berikutnya
- Adzan otomatis
- Countdown iqamah
- Running text
- Pengaturan jadwal/video/audio
- APK otomatis dibangun oleh GitHub Actions

## Struktur media
Letakkan video di:

`app/src/main/assets/video/`

Contoh:
- `masjid1.mp4`
- `masjid2.mp4`
- `masjid3.mp4`

Letakkan audio adzan di:

`app/src/main/assets/audio/`

Contoh:
- `adzan-subuh.mp3`
- `adzan-dzuhur.mp3`
- `adzan-ashar.mp3`
- `adzan-maghrib.mp3`
- `adzan-isya.mp3`

## Build di GitHub
Setiap push ke branch `main` akan menjalankan:

**GitHub Actions → Build APK → Artifact → GitHub Release**

APK hasil build bernama:

`Masjid_Nurul_Amal.apk`

## Build di Android Studio
1. Open folder project.
2. Pastikan JDK 17.
3. Sync Gradle.
4. Run atau pilih **Build → Build APK(s)**.

## Catatan
Workflow menggunakan Gradle 8.10 yang disiapkan oleh GitHub Actions, sehingga repository tidak membutuhkan file binary `gradle-wrapper.jar`.


# DIAGRAM ALUR CI/CD SEDERHANA

## Pipeline CI/CD menggunakan GitHub Actions

```mermaid
flowchart TD
    A["Developer"] --> B["GitHub Repository"]
    B --> C["GitHub Actions"]
    C --> D["Build Aplikasi"]
    D --> E["Test Aplikasi"]
    E --> F{"Test Berhasil?"}
    F -->|Ya| G["Deploy Aplikasi"]
    F -->|Tidak| H["Perbaikan Kode"]
    H --> B
    G --> I["Production"]
    I --> J["Aplikasi Berjalan"]

    style A fill:#dbeafe,stroke:#2563eb
    style B fill:#f3e8ff,stroke:#9333ea
    style C fill:#dbeafe,stroke:#2563eb
    style D fill:#dcfce7,stroke:#16a34a
    style E fill:#dcfce7,stroke:#16a34a
    style G fill:#dcfce7,stroke:#16a34a
    style I fill:#bbf7d0,stroke:#16a34a
```

## Penjelasan

1. Developer membuat kode program.
2. Kode dikirim ke GitHub.
3. GitHub Actions menjalankan pipeline.
4. Build digunakan untuk membangun aplikasi.
5. Test digunakan untuk menguji aplikasi.
6. Deploy mengirim aplikasi ke server.
7. Aplikasi siap digunakan.

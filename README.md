# BL TTHS updates

Repo này dùng để phát hành **artifact update public** cho launcher local-user.

## Mục tiêu

- source repo vẫn có thể giữ private
- launcher chỉ cần một endpoint public để:
  - đọc `latest.json`
  - tải file update `.zip`

## Cấu trúc tối thiểu

- `latest.json`
- `.nojekyll`
- GitHub Releases chứa:
  - `BL-TTHS-Local-macOS-arm64.zip`
  - `BL-TTHS-Local-macOS-x64.zip`
  - `BL-TTHS-Local-windows-x64.zip`

## Khuyến nghị

- bật GitHub Pages cho repo này
- publish `latest.json` từ branch mặc định hoặc thư mục Pages
- dùng GitHub Releases để host file zip theo từng version

## Ví dụ URL

Nếu repo là `org/bl-tths-updates`:

- manifest:
  - `https://org.github.io/bl-tths-updates/latest.json`
- artifact:
  - `https://github.com/org/bl-tths-updates/releases/download/v0.1.1/BL-TTHS-Local-macOS-arm64.zip`
  - `https://github.com/org/bl-tths-updates/releases/download/v0.1.1/BL-TTHS-Local-macOS-x64.zip`
  - `https://github.com/org/bl-tths-updates/releases/download/v0.1.1/BL-TTHS-Local-windows-x64.zip`

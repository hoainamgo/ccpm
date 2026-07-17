# hoainamgo/ccpm (fork) — Podcast 1M Management Layer

[![Agent Skills](https://img.shields.io/badge/Agent_Skills-compatible-4b3baf)](https://agentskills.io)
[![GitHub Issues](https://img.shields.io/badge/+-GitHub%20Issues-1f2328)](https://github.com/hoainamgo/ccpm)

> Fork từ [automazeio/ccpm](https://github.com/automazeio/ccpm) — tùy biến thành **hệ thống quản lý podcast 1 triệu follow, đa nền tảng**.

CCPM gốc biến GitHub Issues thành database quản lý dự án (PRD → Epic → Issue).
Ở fork này, mình giữ nguyên engine, chỉ đổi **quy trình + templates** sang vận hành podcast.

---

## 🎯 Mục tiêu
Quản lý 1 show podcast hướng 1.000.000 follow trên nhiều nền tảng:
YouTube · Spotify · Apple Podcasts · TikTok · Reels · Web.

Hub duy nhất = GitHub Issues + Project Board. Không lưu audio/video ở repo (nặng),
chỉ lưu metadata + link Drive/Obsidian.

## 🧱 Cấu trúc
- `skill/` — CCPM agent skill gốc (giữ nguyên, dùng để sinh kế hoạch).
- `.github/ISSUE_TEMPLATE/` — 3 template: Tập chính | Clip repurpose | Cross-post.
- `docs/workflow.md` — quy trình 9 cột board.
- `docs/labels.md` — danh sách nhãn nền tảng / định dạng / trạng thái.
- `README.md` — file này.

## 🏷️ Labels (tạo thủ công trên repo)
Nền tảng: `platform-youtube` `platform-spotify` `platform-apple` `platform-tiktok` `platform-reels` `platform-web`
Định dạng: `format-full` `format-clip` `format-short`
Trạng thái: `status-ideation` `status-scripting` `status-recording` `status-editing` `status-packaging` `status-scheduling` `status-published` `status-repurpose` `status-analytics`
Vai trò: `role-host` `role-editor` `role-social` `role-analyst`

## 🔄 Quy trình 1 tập (9 cột Board)
Ideation → Scripting → Recording → Editing → Packaging → Scheduling → Published → Repurpose → Analytics

## 🤖 Dùng với Claude Code
1. Cài skill `ccpm` vào Claude Code (copy folder `skill/` vào repo skills của anh).
2. Gõ: "Lên kế hoạch 4 tập tháng 7, mỗi tập đăng YouTube + Spotify + 3 clip TikTok".
3. Claude sinh PRD → Epic → Issues, gắn nhãn tự động.

## 📊 Chỉ số hướng 1 triệu (cột Analytics)
Sub từng nền tảng · view/nghe · retention · engagement (comment/share) · cross-platform conversion.

---
Fork gốc: MIT License. Tùy biến thêm cho podcast — thoải mái dùng nhé 🦷

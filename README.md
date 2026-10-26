# KQK — DQN endgame chess agent

Dự án huấn luyện tác tử DQN chơi cờ tàn cuộc Vua + Hậu vs Vua.

## Cấu trúc

- kqk.ipynb — Môi trường KQK bản mới (có defender, D4 augmentation, 6 kênh)
- kqk_baseline.ipynb — Môi trường KQK bản cũ dùng cho baseline
- train_baseline_L0.ipynb — Huấn luyện giai đoạn 1 (chỉ L0)
- training_agent_final_v2.ipynb — Huấn luyện giai đoạn 2 (curriculum + defender)
- bao_cao_giua_ki_v2.docx — Báo cáo giữa kỳ

## Cách chạy

1. Mở các notebook trên Google Colab, bật T4 GPU.
2. Mount Google Drive.
3. Tạo thư mục KHDL/checkpoints/ và KHDL_baseline/checkpoints/ trên Drive.
4. Chạy theo thứ tự: baseline trước, levelA sau.

## Kết quả

- Baseline L0: 98,4% chiếu hết L0, 70,4% L2.
- LevelA: 100% L2 với defender minimax độ sâu 3 kết hợp luật tránh lặp.

# VNJPTranslate: Hệ thống dịch Việt - Nhật, thiết kế cho dịch thuật quy mô lớn

## 🌟 Mục Lục
1. [Tổng Quan](#tong-quan)
2. [Bộ Dữ Liệu](#bo-du-lieu)
3. [Báo Cáo](#bao-cao)
4. [Mô Hình](#mo-hinh)
5. [English README](https://github.com/ToJupiter/VN-JP-Translate/blob/main/README_EN.md)

---

## 🌟 Tổng Quan <a name="tong-quan"></a>

VNJPTranslate là hệ thống gồm một bộ dataset Việt - Nhật với 3,3 triệu dòng (lớn nhất trong các dataset hiện có), có khả năng tự mở rộng về số lượng và chất lượng cùng với một mô hình nhỏ được fine-tune bằng LoRa để dịch thuật số lượng lớn giữa 2 ngôn ngữ Việt - Nhật. Chi phí tạo sinh và chạy mô hình được tối ưu (với các GPU nhỏ và miễn phí trên Colab và Kaggle).

---

## 📊 Bộ Dữ Liệu <a name="bo-du-lieu"></a>

Bộ dữ liệu VNJPTranslate, bao gồm:

- **3,3 triệu cặp câu song ngữ**, được thu thập từ các nguồn uy tín như Wikipedia tiếng Nhật và tập dữ liệu LLM tiếng Nhật.

- **Tải bộ dữ liệu trên HuggingFace**: [VNJPTranslate Corpus trên Hugging Face](https://huggingface.co/datasets/haiFrHust/VNJPTranslate)

---

## 📝 Báo Cáo <a name="bao-cao"></a>

Để tìm hiểu chi tiết về phương pháp và quy trình, hãy đọc báo cáo trên arXiv nhé
- **Báo cáo**: [Báo cáo VNJPTranslate](https://arxiv.org/abs/2504.00339)

---

## 🚀 Mô Hình <a name="mo-hinh"></a>

- **Mô hình Cơ bản**: Xây dựng trên kiến trúc Qwen 2.5 và được tinh chỉnh bằng:
  - Kỹ thuật Chain-of-Thought - CoT.
  - Hai bộ dữ liệu bổ sung: phiên bản tiếng Việt của Alpaca và bộ dữ liệu câu hỏi - trả lời tiếng Nhật từ Hugging Face.
  
- Dưới đây là mô hình cơ bản, mô hình đạt điểm cao sẽ được cải tiến thêm trong thời gian tới!
 + **Liên kết mô hình**: [Mô hình Cơ bản trên Hugging Face](https://huggingface.co/haiFrHust/VNJPTranslate_base)

- **Hiệu suất mô hình tốt nhất**: Đạt BLEU **28,3** trên tập kiểm tra Tatoeba, vượt qua 20,3 của Opus-MT-Ja-Vi.

Chúng tôi không ngừng cải tiến mô hình để đảm bảo chúng luôn nhẹ và hiệu quả cao.

---

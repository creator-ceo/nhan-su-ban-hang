# nhan-su-ban-hang

**Vai Bán hàng trong đội nhân sự A.I** — của [Tô Hải Đoàn](https://www.facebook.com/tohaidoan/).

> **Phiên bản:** `1.1.0` · 2026-09-07 · giấy phép MIT

---

## ⚠️ Đọc trước: vai này KHÔNG viết hộ bạn

Nó không viết trang bán, không viết chuỗi email, không viết kịch bản gọi. **Nó nghĩ.** Bốn việc:

| Nó làm | |
|---|---|
| **Hỏi cửa phễu TRƯỚC khi hỏi sản phẩm** | Cùng một người, vào bằng cửa khác nhau thì phải bán thứ khác nhau |
| **Soi phễu** | Từng chặng trỏ vào tài sản có hay trống |
| **Chẩn chỗ đứt** | Người rơi ở chặng nào, vì sao |
| **Giữ bốn luật cứng** | Về cách nói giá, hạn chót, con số, giọng chốt — cái nào cũng đã có người trả giá |

📌 **Vai không đẻ tài sản mà vẫn đáng cài, vì nó chặn đúng thứ đắt nhất.** Viết một trang bán rất hay cho sai cửa phễu thì công viết đổ sông — mà lỗi đó chỉ lộ ra sau khi đã đăng. Bước 0 của nó mất một câu hỏi.

Chữ nghĩa thật thì nó giao sang vai Content: `/viet-content` việc `trang-ban-hang`.

## Cài

```bash
claude plugin marketplace add creator-ceo/nhan-su-ban-hang
```

```bash
claude plugin install ban-hang
```

## Lần chạy đầu — dựng hai trang của vai này

| Trang | Là gì |
|---|---|
| **`pheu`** | ⚡ Quan trọng nhất. Bốn chặng · cửa vào nào bán gì · phễu giá cao khác phễu chủ lực ở đâu · chặng nào đang đứt |
| `positioning` | Vì sao chọn bạn chứ không phải người khác, nói bằng một câu |

⚠️ **Chưa có `pheu` thì mọi câu trả lời của vai này đều là đoán.** Nó là trang quyết định mọi tài sản còn lại.

## Việc nào có skill, việc nào chưa

| Việc | Ai làm | Có chưa |
|---|---|---|
| Soi phễu · chẩn chỗ đứt · chọn sản phẩm theo cửa vào | **vai này** | ✅ |
| Viết nội dung trang bán | vai Content → `/viet-content` | ✅ kho `nhan-su-content` |
| Thiết kế offer · chuỗi email · kịch bản gọi 1-1 · offer cho tệp mới · mổ phễu hình mẫu | — | ⬜ chưa có skill |

⚡ **Việc ⬜ thì vai này HƯỚNG DẪN LÀM TAY, không giả vờ chạy.** Nó nói thẳng chưa có skill, rồi đi cùng bạn từng bước — hỏi từng thứ cần, chỉ chỗ nào trong kho đã có, chỗ nào còn trống. Thà chậm mà đúng còn hơn nhận về một bản nghe xuôi tai mà sai cấu trúc.

## ⚠️ Cần cái nền chạy trước

```bash
git clone https://github.com/creator-ceo/nhan-su-thu-thu.git
```

Vai này đọc `offer-ladder` và `target-customer` — hai trang do `/onboard` của nền dựng. Chưa có nền thì nó chạy trên hư không: không biết bạn bán gì, cho ai, giá bao nhiêu.

## Vai này nằm ở đâu trong đội

| Vai | Kho | |
|---|---|---|
| 🧑‍🏫 **Thủ thư** — cái nền, cài trước tiên | `creator-ceo/nhan-su-thu-thu` | ✅ |
| ✍️ **Content** | `creator-ceo/nhan-su-content` | ✅ |
| 🎛️ **Điều phối** | `creator-ceo/nhan-su-dieu-phoi` | ✅ |
| 💰 **Bán hàng** | `creator-ceo/nhan-su-ban-hang` | ✅ **kho này** |
| 🎨 Thiết kế · 🤝 Chăm sóc · 🔍 Nghiên cứu | — | ⬜ chưa |

---

## Ai làm cái này

**Tô Hải Đoàn** — người làm nội dung và xây thương hiệu cá nhân tại Việt Nam. Bốn luật cứng trong đây không phải ý thích: mỗi luật là một lần tôi hoặc người tôi hướng dẫn đã trả giá.

**Kẹt ở đâu thì nhắn tôi:** [facebook.com/tohaidoan](https://www.facebook.com/tohaidoan/)

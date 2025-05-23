# 📌 QUY TRÌNH XÂY DỰNG WEBSITE: NHÀ THẦU VÀ VẬT LIỆU XÂY DỰNG

## 1. KHOI DONG DU AN
| Hạng mục | Mô tả |  |  |  |
| --- | --- | --- | --- | --- |
| 1.1 Xác định mục tiêu | Phục vụ khách hàng có nhu cầu xây nhà, chọn vật liệu, thiết kế ý tưởng – công ty là nhà thầu chính kiêm bán vật liệu. |  |  |  |
| 1.2 Xác định đối tượng người dùng | Người cần xây nhà, người bán vật tư, kỹ sư thi công, kiến trúc sư nội bộ, đối tác nội thất. |  |  |  |
| 1.3 Họp kickoff | Triển khai họp nội bộ, phân vai ban đầu: quản lý dự án, kỹ thuật, thiết kế, nội dung, QA. |  |  |  |

## 2.1 PHAN TICH CHUC NANG
| Module chính | Tính năng con | Đội phụ trách |  |  |
| --- | --- | --- | --- | --- |
| Thiết kế nhà bằng AI | Upload ý tưởng, AI gợi ý mẫu nhà, AI ước lượng chi phí, AI gợi ý vật liệu, gợi ý đối tác nội thất | AI/Backend |  |  |
| Mua vật liệu | Tìm kiếm sản phẩm, phân loại, giỏ hàng, đặt hàng, liên kết với kho | Frontend + Backend |  |  |
| Gói xây dựng | Chọn gói, yêu cầu tư vấn, nhận file thiết kế, theo dõi tiến độ | Backend |  |  |
| Tiến độ công trình | Kỹ sư cập nhật ảnh, ghi chú, tiến độ, khách hàng xem theo thời gian thực | Backend |  |  |
| Đánh giá ẩn danh | Cho phép khách đăng bài, đánh giá dịch vụ nhưng ẩn thông tin, ngoại trừ tên | Frontend + Backend |  |  |
| Tài khoản/Đăng nhập | Khách, Admin, Thiết kế & Thi công, Quản trị viên | Backend |  |  |
| Liên hệ | Quản lí liên hệ của khách hàng | Backend |  |  |

## 2.2 KE HOACH KY THUAT
| Mục | Nội dung |  |  |  |
| --- | --- | --- | --- | --- |
| Frontend | React + CSS + JS + HTML |  |  |  |
| Backend | Spring Boot (Java) |  |  |  |
| Database | MySQL, Redis (caching tiến độ) |  |  |  |
| AI | Google Studio AI, có thể huấn luyện custom |  |  |  |
| Lưu trữ ảnh | Firebase Storage|  |  |  |
| Realtime | Socket.IO (Node) hoặc WebSocket (Spring) |  |  |  |
| Hosting | Frontend: Vercel – Backend: Render/AWS |  |  |  |

## 2.3 TIEN DO VA RUI RO
| Hạng mục | Chi tiết |  |  |  |
| --- | --- | --- | --- | --- |
| WBS | Phân nhóm công việc cho các nhóm: UI/UX, Frontend, Backend, AI, QA |  |  |  |
| Gantt chart | Lập tiến độ từng tuần: Wireframe → UI → API → Tích hợp → Kiểm thử → Triển khai |  |  |  |
| Rủi ro | AI trả lời sai, tốc độ chậm, sản phẩm tải lâu, lỗi thanh toán... |  |  |  |

## 3.1 WIREFRAME
| Trang | Mục đích |  |  |  |
| --- | --- | --- | --- | --- |
| Trang chủ | Tóm tắt dịch vụ, CTA chính |  |  |  |
| Trang Thiết kế AI | Form nhập yêu cầu + kết quả AI + gợi ý vật liệu |  |  |  |
| Trang vật liệu | Danh mục, tìm kiếm, giỏ hàng |  |  |  |
| Trang tiến độ | Khách xem ảnh & trạng thái từng hạng mục |  |  |  |
| Trang đánh giá | Đăng bài, bình luận, ẩn tên |  |  |  |

## 3.2 GIAO DIEN CHI TIET
| Yêu cầu | Ghi chú |  |  |  |
| --- | --- | --- | --- | --- |
| Thiết kế mobile first | Trên 70% người dùng dùng điện thoại |  |  |  |
| Sử dụng màu ngành | Xanh dương (xây dựng), cam/xám (vật liệu), trắng nền |  |  |  |
| Tạo prototype tương tác | Mô phỏng đăng ký, mua hàng, xem AI trả về |  |  |  |

## 4.1 FRONTEND
| Nội dung | Ghi chú |  |  |  |
| --- | --- | --- | --- | --- |
| Tạo cấu trúc project Next.js | pages, components, layouts, utils |  |  |  |
| Giao diện responsive | TailwindCSS |  |  |  |
| Tích hợp AI API | Gửi dữ liệu từ form đến AI, hiển thị kết quả |  |  |  |
| Giao diện theo dõi tiến độ | Timeline, ảnh thực tế từ kỹ sư |  |  |  |

## 4.2 BACKEND
| API chính | Mô tả |  |  |  |
| --- | --- | --- | --- | --- |
| Auth | Đăng ký, đăng nhập, phân quyền |  |  |  |
| AI | Nhận dữ liệu đầu vào → gọi OpenAI → trả kết quả |  |  |  |
| Sản phẩm vật liệu | CRUD sản phẩm, lọc tìm kiếm, giỏ hàng |  |  |  |
| Gói thi công | Tư vấn, đặt lịch hẹn |  |  |  |
| Cập nhật tiến độ | Upload ảnh + ghi chú theo mốc thời gian |  |  |  |

## 4.3 TICH HOP
| Hạng mục | Nội dung |  |  |  |
| --- | --- | --- | --- | --- |
| Kết nối Frontend ↔ Backend | qua API |  |  |  |
| Tích hợp thanh toán | nếu cần |  |  |  |
| Gửi email | xác nhận đơn hàng |  |  |  |
| Gửi push notification | Zalo OA / Email |  |  |  |

## 5. KIEM THU
| Kiểu test | Mục tiêu | Công cụ |  |  |
| --- | --- | --- | --- | --- |
| Manual | Chức năng & UI | TestRail |  |  |
| Tự động hóa | Giao diện, luồng chính | Cypress |  |  |
| Kiểm thử AI | Test dữ liệu đầu vào đa dạng | Thủ công |  |  |
| UAT | Nghiệm thu nội bộ & khách | Checklist có điểm |  |  |

## 6. TRIEN KHAI
| Nội dung | Công cụ |  |  |  |
| --- | --- | --- | --- | --- |
| Triển khai staging | Vercel / Railway |  |  |  |
| Gắn domain, SSL | Cloudflare |  |  |  |
| Backup dữ liệu định kỳ | pg_dump / Firebase rules |  |  |  |

## 7. BAO TRI
| Hạng mục | Nội dung |  |  |  |
| --- | --- | --- | --- | --- |
| Theo dõi lỗi | Sentry, Analytics |  |  |  |
| Thu thập phản hồi | người dùng |  |  |  |
| Cập nhật AI | cập nhật đơn giá vật liệu định kỳ |  |  |  |

## 8. CHIA DOI NGU
| Bộ phận | Trách nhiệm chính |  |  |  |
| --- | --- | --- | --- | --- |
| Product Owner | Quản lý yêu cầu, nghiệp vụ |  |  |  |
| UI/UX | Wireframe, Prototype, Design System |  |  |  |
| Frontend Dev | Giao diện, kết nối API |  |  |  |
| Backend Dev | Logic, AI, database |  |  |  |
| AI Engineer | Tối ưu phản hồi AI |  |  |  |
| QA Tester | Test toàn bộ tính năng |  |  |  |
| DevOps | Deploy, backup, giám sát |  |  |  |

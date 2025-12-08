---
title: "Workshop"
weight: 5
chapter: false
pre: " <b> 5. </b> "
---

{{% notice warning %}}
⚠️ **Lưu ý:** Các thông tin dưới đây chỉ nhằm mục đích tham khảo, vui lòng **không sao chép nguyên văn** cho bài báo cáo của bạn kể cả warning này.
{{% /notice %}}

# Truy cập Hybrid an toàn đến S3 sử dụng VPC Endpoints

#### Tổng quan

**AWS PrivateLink** cung cấp kết nối riêng tư đến các dịch vụ AWS từ VPCs và mạng on-premises của bạn, mà không để lộ lưu lượng truy cập ra Internet công cộng.

Trong bài lab này, bạn sẽ học cách tạo, cấu hình và kiểm tra VPC endpoints cho phép các workload của bạn truy cập các dịch vụ AWS mà không cần đi qua Internet công cộng.

Bạn sẽ tạo hai loại endpoints để truy cập Amazon S3: Gateway VPC endpoint và Interface VPC endpoint. Hai loại VPC endpoints này cung cấp các lợi ích khác nhau tùy thuộc vào việc bạn truy cập Amazon S3 từ cloud hay từ vị trí on-premises của bạn.

- **Gateway** - Tạo gateway endpoint để gửi lưu lượng đến Amazon S3 hoặc DynamoDB sử dụng địa chỉ IP riêng tư. Bạn định tuyến lưu lượng từ VPC của bạn đến gateway endpoint bằng cách sử dụng bảng định tuyến (route tables).
- **Interface** - Tạo interface endpoint để gửi lưu lượng đến các dịch vụ endpoint sử dụng Network Load Balancer để phân phối lưu lượng. Lưu lượng hướng đến dịch vụ endpoint được phân giải bằng DNS.

#### Nội dung

1. [Tổng quan Workshop](5.1-Workshop-overview)
2. [Chuẩn bị](5.2-Prerequiste/)
3. [Truy cập S3 từ VPC](5.3-S3-vpc/)
4. [Sử dụng SES](5.4-SES/)
5. [Sử dụng Route53](5.5-Route53/)
6. [Dọn dẹp tài nguyên](5.6-Cleanup/)
7. [Sử dụng S3](5.7-S3/)

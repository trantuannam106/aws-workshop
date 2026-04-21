---
title: "Worklog Tuần 1"
date: 2026-04-20
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---
### Mục tiêu tuần 1:

* Làm quen với môi trường thực tập và các thành viên trong chương trình First Cloud Journey.
* Nắm được khái niệm cơ bản về Cloud Computing và hệ sinh thái dịch vụ AWS.
* Làm quen với AWS Management Console và AWS CLI.
* Thực hành triển khai và quản lý tài nguyên cơ bản trên AWS (EC2, EBS).

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Làm quen với các thành viên FCJ <br> - Đọc và lưu ý các nội quy, quy định tại đơn vị thực tập                                                                                             | 20/04/2026   | 20/04/2026      |
| 3   | - Tìm hiểu AWS và các loại dịch vụ <br>&emsp; + Compute <br>&emsp; + Storage <br>&emsp; + Networking <br>&emsp; + Database <br>&emsp; + ... <br>                                            | 21/04/2026   | 21/04/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Tạo AWS Free Tier account <br> - Tìm hiểu AWS Console & AWS CLI <br> - **Thực hành:** <br>&emsp; + Tạo AWS account <br>&emsp; + Cài AWS CLI & cấu hình <br> &emsp; + Cách sử dụng AWS CLI | 22/04/2026   | 22/04/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - Tìm hiểu EC2 cơ bản: <br>&emsp; + Instance types <br>&emsp; + AMI <br>&emsp; + EBS <br>&emsp; + ... <br> - Các cách remote SSH vào EC2 <br> - Tìm hiểu Elastic IP   <br>                  | 23/04/2026   | 23/04/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - **Thực hành:** <br>&emsp; + Tạo EC2 instance <br>&emsp; + Kết nối SSH <br>&emsp; + Gắn EBS volume                                                                                         | 24/04/2026   | 24/04/2026      | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 1:

#### Kiến thức

* Hiểu được khái niệm Cloud Computing và vai trò của AWS.
* Nắm được các nhóm dịch vụ chính:
  * Compute (EC2)
  * Storage (S3, EBS)
  * Networking (VPC, Security Group)
  * Database (RDS)
* Hiểu mối liên hệ giữa các dịch vụ trong hệ thống cloud.

---

#### Thực hành

* Tạo thành công AWS Free Tier account.
* Làm quen với AWS Management Console:
  * Tìm kiếm và truy cập dịch vụ
  * Quản lý tài nguyên

* Cài đặt và cấu hình AWS CLI:
  * Access Key
  * Secret Key
  * Default Region

* Thực hiện các lệnh cơ bản:
  * ```bash
  * aws configure list
  * aws ec2 describe-instances
  * aws ec2 describe-regions

* Triển khai EC2:

* Tạo 01 EC2 instance (t2.micro - Free Tier)
  * Tạo và sử dụng key pair (.pem)
  * Kết nối SSH thành công vào instance

* Làm việc với EBS:
  * Tạo EBS volume (8GB)
  * Attach vào EC2 instance
  * Kiểm tra và mount volume

* Có khả năng sử dụng song song:
  * AWS Console (GUI)
  * AWS CLI

---

#### Khó khăn và cách giải quyết
* Khó khăn
  * Lỗi khi SSH vào EC2 (Permission denied).
  * Chưa hiểu rõ Security Group hoạt động như thế nào.
  * Nhầm lẫn region khi cấu hình AWS CLI.
* Cách giải quyết

Cấp quyền cho file key:
```bash
  chmod 400 key.pem
```

* Đọc tài liệu và thực hành lại nhiều lần để hiểu Security Group.
* Cấu hình lại CLI:
```bash
  aws configure
```

---

#### Minh chứng
* AWS Console (EC2 instance running)
* Terminal SSH thành công
* Kết quả lệnh AWS CLI
* EBS volume đã attach

Ví dụ:

![EC2 Instance](../images/ec2-instance.png)
![SSH EC2](../images/ssh-ec2.png)

---

#### Bài học rút ra
* Hiểu rõ hơn về mô hình Cloud (IaaS).
* Làm quen với việc quản lý tài nguyên từ xa.
* Biết cách xử lý lỗi khi làm việc với hệ thống mới.
* Nhận thấy sự khác biệt giữa local và cloud environment.

---

#### Định hướng tuần tiếp theo
* Tìm hiểu AWS Networking (VPC, Subnet).
* Làm việc với S3.
* Deploy một ứng dụng đơn giản lên EC2.
Mobile Learning-sandbox day 2
==================================
## 1. Clone project
```sh
git clone https://github.com/songoku14/NALDay2Demo.git
```
## 2. Lấy code từ develop branch 
- Để lấy code từ develop bạn cần chuyển sang branch develop và pull code về.
- Kiểm tra xem mình đang ở branch nào
```sh
git branch
```
- Tạo branch develop 
```sh
git branch develop
```
- Chuyển sang branch develop 
```sh
git checkout develop
```
- Lấy code từ  remote branch develop trên server
```sh
git pull origin develop
```
## 3. Viết code của bạn 
- Bây giờ bạn cần chỉnh sửa file NALInfo.md  để viết thông tin của bạn vào.
- Trước hết cần tạo  feature branch 
```sh
git branch change_your_name
```
- Chuyển sang branch vừa tạo
```sh
git checkout change_your_name
```
- Mở file NALInfo.md
```sh
vim NALInfo.md
```
- Ấn "i" để  insert, sau khi điền thông tin của bạn vào phần 4. Giới thiệu bản thân nhấn "ESC" để thoát và ":wq" để lưu thông tin.
- Kiểm tra những thay đổi của bạn  bằng cách sử dụng lệnh 
```sh
git status
```
- add file NALInfo.md để lưu lại những thay đổi.
```sh
git add NALInfo.md
```
- commit sự thay đổi đấy.
```sh
git commit -m "update my name"
```
- Như vậy bạn đã lưu thay đổi đấy vào  local branch change_your_name.
## 4. Đẩy code mới lên develop
- Bây giờ chúng ta sẽ đẩy thông tin này lên remote develop branch
- Chuyển sang branch develop
- Sử dụng câu lệnh merge để merge branch change_your_name  vào  develop
```sh
git merge change_your_name
```
- Như vậy develop đã có code mới của branch change_your_name. Nhưng thay đổi này mới chỉ được thực  hiện dưới local của bạn. Để public ra cho tất cả mọi người trong team cùng biết, ta cần đẩy thay đổi lên remote develop branch.
```sh
git push origin develop
```










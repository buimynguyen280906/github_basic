# Git hub cơ bản

## Github là gì
- github là công cụ để những người lập trình viên có thể lưu trữ quản lí và hợp tác với nhau làm chung một dự án , hỗ trợ người lập trình có thể kiểm tra quản lí dự án trong quá trình làm việc .
  
## Lợi ích khi sử dụng github

### quản lí source code dễ dàng
 - khi tạo 1 cái repo thì toàn bộ cái source code đc lưu trên github . ở đây mình có thể coi lại quá trình làm việc thông qua các comment sau mỗi lần commit . và nhiều người cũng có thể làm cùng 1 cái repo
 - mình có thể kiểm tra ai đã commit và commit những gì .
 - khi tạo 1  nhánh master thì mình có thể phát triển  thêm nhiều nhánh trên 1 nhánh chính , cuối cùng cần phải hợp nhất những nhánh đó lại vào nhánh master để ra được một project hoàn chỉnh
 ### Tracking sự thay đổi qua các version 
 - khi có nhiều thành viên cùng tham gia một dự án thì khó có thể quản lí hết vì thế github là nơi sẽ lưu lại hết những thay đổi mà thành viên đó đã push lên repository . để phòng trường hợp bị mất các thay đổi trước đó chưa được lưu. 
 
 ## Các câu lệnh thông dụng
 ### git init 
 - dùng để khởi tạo một repository git mới hoặc bắt đầu quản lí phiên bản mã nguồn của một dự án từ đầu , khi bắt đầu chạy git init , Git sẽ tạo ra thư mục .git ẩn trong thư mục dự án của bạn chứa toàn bộ hệ thống quản lí phiên bản git và lịch sử thay đổi
 
 ### git add 
 - git add là một trong những lệnh qtrong trong git , được sử dụng để thêm (add) các tệp các thư mục đã thay đổi vào vùng chờ (staging area) để chuẩn bị cho việc tạo commit : 
  + git add . hoặc git add *  sử dụng để thêm tất cả các thư mục đã thay đỏi hoặc trong thư mục hiện tại vào vùng chờ.
  + git add -u hoặc git add --update : sử dụng để thêm tất cả các tệp đã thay đổi( nhưng không bao gồm các tệp mới ) vào vùng chờ

  ### git commit 
  - dùng để mô tả sự thay đổi của một repository cùng với mô tả sự thay đổi của các thay đổi đó 
  - mô tả commit cần rõ ràng , ngắn gọn chỉ ra lí do của sự thay đổi và sử dụng [ tag ] như feat( tính năng mới) , fix(sửa ) , refactor ( tái cấu trúc ) , docs(thêm tài liệu)....
  ### git push 
  - được dùng để đẩy các commit và thay đổi từ máy tính của bạn lên một remote repository , thường là một dịch vụ như github , hoặc một máy chủ git từ xa , lệnh này có nhiệm vụ cập nhật repository từ xa với các thay đổi mới nhất từ nhánh hiện tại của bạn .
  - tên-remote thường là repository từ xa 
  - tên-nhánh là tên của nhánh mà bạn muốn đẩy lên repository từ xa 
  ### git pull
  - là một lệnh trong git được sử dụng để cập nhật mã nguồn của bạn từ một repositoryb từ xa , lệnh này có nhiệm vụ gộp (merge) các thay đổi từ repository từ xa vào branch hiện tại của bạn và đồng thời có thể tải về bất kì thay đổi mới nào từ repository từ xa. 
   khi tải vèe các repository từ xa git sẽ tự động thao tác gộp để kết hợp các thay đổi này vào branch hiện tại , trong trường hợp sảy ra xung đột (conflict) bạn cần giả quyết xung đột trước khi commit 
   ### git checkout 
 được dùng để thực hiện nhiều chức năng khác nhau như chuyển đổi giữa các nhánh , tạo nhánh mới hoặc thay đổi trạng thái  làm viêcj với file cụ thể :
 -  chuyển đỏi giữa các nhánh : khi bạn chạy git checkour với tên branch , bạn đang chuyển đổi từ một branch sang nhánh khác , điều này cho phép bạn đang làm việc trên một branch cụ thể của dự án  
 -  tạo nhánh mới và chuyển đổi lên nhánh đó : bằng cách dùng lệnh (git checkout -b [tên-nhánh ]) 
 - chuyển đổi đến phiên bản cụ thể : chuyển đến một phiên bản cụ thể của file hoặc forder trong lịch sử commit 
 - chuyển đổi giữa trạng thái làm việc với file : nếu bạn sử dụng git add để đưa tệp vào vùng chờ và muốn hoàn tác (unstage) chúng, bạn có thể sử dụng git checkout -- [tên tệp ] để loại bỏ tệp đó khỏi vùng chờ - chuyển đổi đến thẻ (tags) : bạn cũng có thể sử dụng git checkout để chuyển đổi đến một thẻ cụ thể (tag) trong dự án , giống như bạn chuyển đổi đến một commit cụ thể .
 ### git status 
hiện thị thông tin khác nhau (do thêm mới, xóa đi, sửa đổi các file) giữa các file trong các trường hợp:
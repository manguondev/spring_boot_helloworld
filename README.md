# spring_boot_helloworld
## Hướng dẫn khởi tạo ứng dụng HelloWorld với Spring Boot

[Spring Boot là gì?](https://manguon.dev/spring-boot-la-gi-tinh-nang-noi-bat-cua-spring-boot/) Spring Boot là một mô đun trong Spring với mục đích cung cấp tính năng RAD (Rapid Application Development – phát triển ứng dụng nhanh) trong hệ sinh thái Spring Framework. Khi xây dựng ứng dụng với Spring Boot sẽ giúp lập trình viên xây dựng các ứng dụng Spring nhanh chóng, giảm thiểu yêu cầu cấu hình XML.

Một trong những cách đơn giản nhất để khởi tạo một ứng dụng Spring Boot bằng cách bạn truy cập vào trang Spring Initializr để khởi tạo tự động.

Bước 1: Khởi tạo ứng dụng HelloWorld với Spring Boot bằng cách vào mục File > New Project…, bạn tìm đến danh mục Maven rồi chọn vào Spring Boot Initializr project.

<img src="https://manguon.dev/wp-content/uploads/2019/06/manguondev-khoi-tao-ung-dung-helloworld-voi-spring-boot-h01.jpg">

Màn hình New Spring Initializr Project bạn cần nhập các thông tin về dự án như Group, Artifact, Package, Version, Name…

<img src="https://manguon.dev/wp-content/uploads/2019/06/manguondev-khoi-tao-ung-dung-helloworld-voi-spring-boot-h02.jpg">

Tiếp theo bạn chọn một số thư viện cần thiết chẳng hạn JPA, Websocket, MySQL…

<img src="https://manguon.dev/wp-content/uploads/2019/06/manguondev-khoi-tao-ung-dung-helloworld-voi-spring-boot-h03-768x500.jpg">

Cuối cùng chọn nơi lưu trữ dự án để kết thúc quá trình khởi tạo ứng dụng HelloWorld với Spring Boot.

<img src="https://manguon.dev/wp-content/uploads/2019/06/manguondev-khoi-tao-ung-dung-helloworld-voi-spring-boot-h04-768x500.jpg">

Bước 2: Tiếp theo bạn tạo controller chẳng hạn HelloWorldController để hiển thị dòng chữ Hello World khi truy cập.

```
package dev.manguon.helloworld.controller;
 
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RestController;
 
/**
 *
 * @author MA NGUON
 */
@RestController
public class HelloWorldController {
 
    @GetMapping("/hello")
    public String sayHello() {
        return "Hello World!";
    }
 
}
```

Bước 3: Bây giờ bạn có thể khởi chạy ứng dụng để kiểm tra kết quả việc khởi tạo ứng dụng HelloWorld với Spring Boot thành công hay chưa.

Mở trình duyệt và truy cập vào đường dẫn http://localhost:8080/hello/

<img src="https://manguon.dev/wp-content/uploads/2019/06/manguondev-khoi-tao-ung-dung-helloworld-voi-spring-boot-h05.jpg">

Tác giả: [manguondev](https://manguon.dev/author/manguondev/)
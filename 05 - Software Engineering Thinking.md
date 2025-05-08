# ✅ 05 - Software Engineering Thinking - Xây Dựng Phần Mềm Chuyên Nghiệp Từ Tư Duy Đến Thực Hành

Chào mừng bạn đến với chương thứ sáu! Sau khi đã nắm vững tư duy hệ thống, làm chủ dòng lệnh Linux, rèn luyện bộ não thuật toán và hiểu sâu sắc về quản lý dữ liệu, giờ đây chúng ta sẽ học cách **hiện thực hóa những ý tưởng thành các sản phẩm phần mềm thực tế**. **Software Engineering Thinking** không chỉ là việc viết code, mà là một quá trình **tư duy có hệ thống** từ khâu thiết kế, phát triển, kiểm thử đến triển khai và bảo trì.

Trong chương này, chúng ta sẽ khám phá những nguyên tắc thiết kế phần mềm đã được kiểm chứng qua thời gian, tìm hiểu về các quy trình phát triển phổ biến, nắm vững các kỹ thuật kiểm thử quan trọng và đặc biệt, chúng ta sẽ **đi sâu vào tư duy lập trình hướng đối tượng (OOP)** - một trong nhữngParadigm lập trình mạnh mẽ và phổ biến nhất. Hãy sẵn sàng để nâng tầm kỹ năng xây dựng phần mềm của bạn lên một đẳng cấp mới!

## 🛠️ Áp dụng nguyên tắc thiết kế phần mềm: SOLID, DRY, KISS

Những nguyên tắc thiết kế phần mềm này là những "kim chỉ nam" giúp bạn viết code sạch, dễ hiểu, linh hoạt và dễ bảo trì:

* **SOLID:** Tập hợp 5 nguyên tắc cơ bản của lập trình hướng đối tượng:
  * **Single Responsibility Principle (SRP - Nguyên tắc đơn trách nhiệm):** Một class chỉ nên có một và chỉ một lý do để thay đổi.
  * **Open/Closed Principle (OCP - Nguyên tắc đóng mở):** Các entity phần mềm (classes, modules, functions,...) nên mở rộng để thay đổi, nhưng đóng lại đối với việc sửa đổi.
  * **Liskov Substitution Principle (LSP - Nguyên tắc thay thế Liskov):** Các subtype phải có khả năng thay thế các base type của chúng mà không làm thay đổi tính đúng đắn của chương trình.
  * **Interface Segregation Principle (ISP - Nguyên tắc phân tách interface):** Không nên ép các client phải phụ thuộc vào các interface mà họ không sử dụng.
  * **Dependency Inversion Principle (DIP - Nguyên tắc đảo ngược phụ thuộc):**
    * Các module cấp cao không nên phụ thuộc vào các module cấp thấp. Cả hai nên phụ thuộc vào các abstraction.
    * Các abstraction không nên phụ thuộc vào details. Details nên phụ thuộc vào abstractions.

* **DRY (Don't Repeat Yourself - Đừng lặp lại chính mình):** Tránh viết cùng một đoạn code ở nhiều nơi khác nhau. Thay vào đó, hãy trừu tượng hóa và tái sử dụng code. Điều này giúp giảm thiểu lỗi, dễ dàng bảo trì và cập nhật code hơn.

* **KISS (Keep It Simple, Stupid - Giữ cho nó đơn giản):** Ưu tiên các giải pháp đơn giản và dễ hiểu hơn là các giải pháp phức tạp không cần thiết. Code đơn giản thường dễ đọc, dễ bảo trì và ít lỗi hơn.

Hiểu và áp dụng những nguyên tắc này sẽ giúp bạn xây dựng những hệ thống phần mềm **mạnh mẽ, linh hoạt và bền vững**.

## 🔄 Hiểu quy trình phát triển phần mềm

Một quy trình phát triển phần mềm rõ ràng giúp đội ngũ phát triển làm việc một cách có tổ chức, hiệu quả và đảm bảo chất lượng sản phẩm. Chúng ta sẽ tìm hiểu về hai mô hình phổ biến:

### 🏃 Agile / Scrum

Đây là một phương pháp phát triển lặp đi lặp lại và tăng trưởng, tập trung vào sự linh hoạt, khả năng thích ứng với thay đổi và sự hợp tác chặt chẽ giữa các thành viên trong nhóm và với khách hàng. Scrum là một framework phổ biến của Agile, với các khái niệm chính như:

* **Sprints:** Các chu kỳ phát triển ngắn (thường từ 1 đến 4 tuần).
* **Product Backlog:** Danh sách tất cả các tính năng, yêu cầu và cải tiến cần thực hiện.
* **Sprint Backlog:** Tập hợp các công việc mà nhóm sẽ thực hiện trong một Sprint.
* **Daily Scrum (Stand-up):** Cuộc họp ngắn hàng ngày để các thành viên chia sẻ tiến độ và các vấn đề gặp phải.
* **Sprint Planning:** Buổi họp đầu Sprint để lên kế hoạch cho các công việc sẽ thực hiện.
* **Sprint Review:** Buổi họp cuối Sprint để trình bày kết quả cho khách hàng và các bên liên quan.
* **Sprint Retrospective:** Buổi họp cuối Sprint để nhóm nhìn lại quá trình làm việc và tìm cách cải thiện.

### ⚙️ DevOps

Đây là một tập hợp các phương pháp thực hành nhằm mục đích **tự động hóa và tích hợp các quy trình giữa phát triển phần mềm (Dev) và vận hành hệ thống (Ops)**. Mục tiêu của DevOps là rút ngắn chu kỳ phát triển, tăng tần suất triển khai, và đảm bảo tính ổn định và tin cậy của hệ thống. Các yếu tố quan trọng của DevOps bao gồm:

* **Continuous Integration (CI - Tích hợp liên tục):** Thường xuyên tích hợp code từ các thành viên trong nhóm vào một repository chung và tự động build, kiểm thử.
* **Continuous Delivery (CD - Phân phối liên tục):** Tự động chuẩn bị code đã được kiểm thử để có thể triển khai lên môi trường dev/ qa/ staging/ production bất cứ lúc nào.
* **Continuous Deployment (CD - Triển khai liên tục):** Tự động triển khai code đã vượt qua kiểm thử lên môi trường production.
* **Infrastructure as Code (IaC):** Quản lý và cấu hình hạ tầng bằng code, giúp tự động hóa và tái sử dụng.
* **Monitoring and Logging:** Theo dõi hiệu suất hệ thống và thu thập log để phát hiện và xử lý sự cố nhanh chóng.

Hiểu các quy trình này giúp bạn làm việc hiệu quả hơn trong các dự án phần mềm và phối hợp tốt hơn với các thành viên khác trong nhóm.

## 🧪 Thực hành kiểm thử

Kiểm thử phần mềm là một quá trình quan trọng để đảm bảo chất lượng, độ tin cậy và tính ổn định của sản phẩm. Chúng ta sẽ tìm hiểu về các loại kiểm thử cơ bản:

* **Unit Test (Kiểm thử đơn vị):** Kiểm thử các đơn vị code nhỏ nhất (thường là các hàm hoặc phương thức) một cách độc lập để đảm bảo chúng hoạt động đúng như mong đợi.
* **Integration Test (Kiểm thử tích hợp):** Kiểm thử sự tương tác giữa các module hoặc các thành phần khác nhau của hệ thống để đảm bảo chúng làm việc cùng nhau một cách chính xác.
* **CI/CD (Continuous Integration/Continuous Delivery or Deployment):** Như đã đề cập ở trên, CI/CD là một quy trình tự động hóa việc build, kiểm thử và triển khai phần mềm, giúp phát hiện lỗi sớm và đưa sản phẩm đến người dùng nhanh hơn.

Thực hành viết unit test và integration test là một kỹ năng không thể thiếu của một Software Engineer chuyên nghiệp. Nó giúp bạn tự tin hơn vào code của mình và giảm thiểu rủi ro phát sinh lỗi trong quá trình phát triển và vận hành.

## 🧱 Thiết kế phần mềm

Thiết kế phần mềm là quá trình xác định cấu trúc, các thành phần và cách chúng tương tác với nhau để đáp ứng các yêu cầu của hệ thống. Chúng ta sẽ tập trung vào hai mô hình thiết kế quan trọng:

### 🎯 Hướng đối tượng (Object-Oriented Programming - OOP)

Đây là một paradigm lập trình dựa trên khái niệm về **đối tượng (objects)**, là các thực thể chứa cả **dữ liệu (attributes)** và **hành vi (methods)**. OOP tập trung vào việc tổ chức code xung quanh các đối tượng và sự tương tác giữa chúng. Bốn trụ cột chính của OOP là:

* **Encapsulation (Tính đóng gói):** Che giấu thông tin bên trong đối tượng và chỉ cho phép truy cập thông qua các phương thức công khai. Điều này giúp bảo vệ dữ liệu và giảm sự phụ thuộc giữa các phần của code.
* **Abstraction (Tính trừu tượng):** Ẩn đi các chi tiết phức tạp và chỉ hiển thị những thông tin cần thiết cho người sử dụng. Điều này giúp làm giảm độ phức tạp và tăng tính dễ hiểu của code.
* **Inheritance (Tính kế thừa):** Cho phép một class (subclass/derived class) kế thừa các thuộc tính và phương thức từ một class khác (superclass/base class). Điều này giúp tái sử dụng code và xây dựng các hệ thống phân cấp class.
* **Polymorphism (Tính đa hình):** Cho phép các đối tượng thuộc các class khác nhau phản ứng theo những cách khác nhau đối với cùng một thông điệp (method call). Điều này mang lại sự linh hoạt và khả năng mở rộng cao cho code.

Hiểu sâu sắc về OOP và cách áp dụng nó trong thiết kế phần mềm là nền tảng để xây dựng các ứng dụng phức tạp và dễ bảo trì.

### 🌐 Hướng dịch vụ (Service-Oriented Architecture - SOA)

Đây là một kiến trúc phần mềm mà các thành phần ứng dụng được cung cấp dưới dạng các **dịch vụ (services)** có thể giao tiếp với nhau thông qua một giao thức mạng (thường là HTTP). SOA tập trung vào việc xây dựng các dịch vụ độc lập, có khả năng tái sử dụng và dễ dàng tích hợp với nhau để tạo thành các ứng dụng lớn và phức tạp. Microservices là một biến thể hiện đại của SOA, tập trung vào việc xây dựng các dịch vụ nhỏ hơn, độc lập hơn và có thể triển khai độc lập.

Hiểu về SOA và Microservices giúp bạn thiết kế các hệ thống phân tán, có khả năng mở rộng và linh hoạt cao.

---

**🎉 Chúc mừng bạn đã hoàn thành chương 05 về Software Engineering Thinking!** Bạn đã trang bị cho mình những kiến thức và tư duy quan trọng để xây dựng phần mềm một cách chuyên nghiệp, từ việc áp dụng các nguyên tắc thiết kế, hiểu các quy trình phát triển, thực hành kiểm thử đến việc nắm vững các mô hình thiết kế phần mềm, đặc biệt là OOP.

**📝 Chuẩn bị cho chương tiếp theo - ✅ 06 - Java Thinking:**

Để chuẩn bị tốt nhất cho chương "Java Thinking", bạn có thể làm quen trước với những điều sau:

* **Ngôn ngữ lập trình Java:** Tìm hiểu về lịch sử, đặc điểm và các ứng dụng phổ biến của Java.
* **Các khái niệm cơ bản của OOP trong Java:** Class, object, thuộc tính, phương thức, kế thừa, đa hình, trừu tượng, đóng gói.
* **Java Virtual Machine (JVM):** Hiểu vai trò của JVM trong việc chạy các ứng dụng Java.
* **Các khái niệm cơ bản về Garbage Collection trong Java.**

Nếu bạn đã có kinh nghiệm với một ngôn ngữ lập trình hướng đối tượng khác, việc tiếp cận Java sẽ dễ dàng hơn. Dành thời gian tìm hiểu về cú pháp và các đặc điểm riêng của Java sẽ giúp bạn bắt đầu chương tiếp theo một cách thuận lợi.

Hẹn gặp lại bạn ở chương 06, nơi chúng ta sẽ đi sâu vào tư duy lập trình với một trong những ngôn ngữ mạnh mẽ và phổ biến nhất thế giới!

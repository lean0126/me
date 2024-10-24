<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Câu hỏi và nút Đồng ý/Không đồng ý</title>
    <style>
        /* Hiệu ứng nền LED */
        @keyframes ledGlow {
            0% { background-color: rgba(255, 0, 0, 0.8); }
            25% { background-color: rgba(0, 255, 0, 0.8); }
            50% { background-color: rgba(0, 0, 255, 0.8); }
            75% { background-color: rgba(255, 255, 0, 0.8); }
            100% { background-color: rgba(255, 0, 255, 0.8); }
        }

        body {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background: linear-gradient(135deg, rgba(255, 204, 203, 0.8), rgba(255, 182, 193, 0.8));
            animation: ledGlow 8s ease infinite; /* Thêm hiệu ứng LED cho nền */
            font-family: Arial, sans-serif;
            position: relative;
            overflow: hidden;
        }

        /* Câu hỏi */
        .question {
            font-size: 24px;
            margin-bottom: 20px;
            color: #333;
            text-shadow: 2px 2px 4px rgba(255, 255, 255, 0.7);
        }

        /* CSS cho phần chứa các nút */
        .button-container {
            display: flex;
            gap: 20px;
        }

        /* CSS cho nút chung */
        .custom-button {
            padding: 15px 32px;
            font-size: 16px;
            cursor: pointer;
            border: none;
            border-radius: 8px;
            color: white;
            transition: background-color 0.3s, transform 0.3s; /* Hiệu ứng chuyển màu và phóng to */
        }

        /* Nút Đồng ý */
        .agree-button {
            background-color: #4CAF50; /* Màu xanh lá */
        }

        /* Nút Không đồng ý */
        .disagree-button {
            background-color: #f44336; /* Màu đỏ */
        }

        /* CSS cho thông điệp sẽ xuất hiện */
        .message {
            display: none; /* Ẩn thông điệp cho đến khi cần hiển thị */
            margin-top: 20px;
            font-size: 20px;
            color: #000; /* Màu chữ cho thông điệp */
        }

        /* CSS cho biểu tượng vui vẻ */
        .happy-icon {
            position: absolute;
            opacity: 0.8;
            width: 50px; /* Kích thước biểu tượng */
            animation: float 5s ease-in-out infinite; /* Hiệu ứng bay xung quanh */
            transition: transform 0.3s ease; /* Hiệu ứng mờ ảo */
        }

        /* Hiệu ứng di chuyển ngẫu nhiên */
        @keyframes float {
            0% { transform: translate(0, 0); }
            25% { transform: translate(-20px, -30px); }
            50% { transform: translate(30px, -20px); }
            75% { transform: translate(-30px, 20px); }
            100% { transform: translate(0, 0); }
        }

        /* CSS cho bông hoa */
        .flower {
            position: absolute;
            bottom: 0; /* Xuất hiện từ dưới cùng */
            width: 50px; /* Kích thước hoa */
            opacity: 0; /* Ẩn hoa ban đầu */
            animation: bloom 1s forwards; /* Hiệu ứng nở hoa */
        }

        /* Hiệu ứng nở hoa */
        @keyframes bloom {
            0% { transform: scale(0); opacity: 1; }
            100% { transform: scale(2); opacity: 0; } /* Bông hoa sẽ phình to và biến mất */
        }

        /* Hiệu ứng biến mất từ từ */
        @keyframes fadeOut {
            0% { opacity: 1; }
            100% { opacity: 0; }
        }

        /* Hiệu ứng khi di chuột vào nút */
        .custom-button:hover {
            transform: scale(1.1); /* Phóng to nút khi di chuột vào */
            background-color: rgba(255, 255, 255, 0.7); /* Thay đổi màu nền khi di chuột */
            color: #333; /* Đổi màu chữ khi di chuột */
        }
    </style>
</head>
<body>

    <!-- Câu hỏi -->
    <div class="question">ĐI CHƠI KHÔNG BÊN ĐÓ?</div>

    <!-- Nút Đồng ý và Không đồng ý -->
    <div class="button-container">
        <button class="custom-button agree-button" onclick="handleAgree()">Đồng ý</button>
        <button class="custom-button disagree-button" id="disagreeButton" onclick="handleDisagree()">Không đồng ý</button>
    </div>

    <!-- Thông điệp sẽ xuất hiện -->
    <div class="message" id="message-container">
        <span>ĐI THÔI 😍</span>
    </div>

    <script>
        // Biến để theo dõi thông điệp
        const messages = [
            "Bấm vào cái xanh ấy!",
            "Xanh ấy, bị cái gì gì!",
            "Xanh kia kìa!",
            "Xợ mà!"
        ];
        let messageIndex = 0; // Chỉ số của thông điệp hiện tại
        let intervalId; // Để lưu trữ ID của interval

        // Xử lý khi bấm nút Đồng ý
        function handleAgree() {
            const messageContainer = document.getElementById('message-container');
            messageContainer.style.display = 'block'; // Hiện thông điệp "Đi thôi!"
            document.getElementById('disagreeButton').style.display = 'none'; // Ẩn nút Không đồng ý
            
            // Tạo các biểu tượng vui vẻ và hoa
            createHappyIcons();
            createFlowers();
        }

        // Xử lý khi bấm nút Không đồng ý
        function handleDisagree() {
            const button = document.getElementById('disagreeButton');

            // Hiển thị thông điệp lần lượt trong nút
            if (messageIndex < messages.length) {
                button.innerText = messages[messageIndex]; // Cập nhật nội dung của nút
                messageIndex++;
                
                // Di chuyển nút Không đồng ý đến vị trí ngẫu nhiên
                setTimeout(() => {
                    const randomX = Math.random() * (window.innerWidth - button.offsetWidth);
                    const randomY = Math.random() * (window.innerHeight - button.offsetHeight);
                    button.style.position = 'absolute'; // Đặt vị trí tuyệt đối
                    button.style.left = `${randomX}px`;
                    button.style.top = `${randomY}px`;
                }, 100); // Thời gian trước khi di chuyển
            } else {
                // Sau khi hiển thị tất cả thông điệp, bắt đầu nhảy loạn xạ
                startMovingRandomly(button);
            }
        }

        // Hàm di chuyển nút Không đồng ý một cách ngẫu nhiên
        function startMovingRandomly(button) {
            // Sử dụng setInterval để thay đổi vị trí và nội dung liên tục
            intervalId = setInterval(() => {
                const randomX = Math.random() * (window.innerWidth - button.offsetWidth);
                const randomY = Math.random() * (window.innerHeight - button.offsetHeight);
                button.style.left = `${randomX}px`;
                button.style.top = `${randomY}px`;

                // Thay đổi chữ trong nút một cách ngẫu nhiên
                button.innerText = messages[Math.floor(Math.random() * messages.length)];
            }, 300); // Thay đổi mỗi 300ms
        }

        // Hàm tạo biểu tượng vui vẻ
        function createHappyIcons() {
            const icons = ["😊", "😍", "🥰", "😻", "💐","💖", "😍", "💕", "🌻", "💗"]; // Danh sách biểu tượng vui vẻ
            for (let i = 0; i < 20; i++) { // Tăng số lượng biểu tượng lên 20
                const icon = document.createElement('div');
                icon.className = 'happy-icon';
                icon.innerText = icons[Math.floor(Math.random() * icons.length)];
                icon.style.left = `${Math.random() * 100}vw`; // Vị trí ngẫu nhiên
                icon.style.top = `${Math.random() * 100}vh`; // Vị trí ngẫu nhiên theo chiều cao
                icon.style.fontSize = `${Math.random() * 30 + 20}px`; // Kích thước ngẫu nhiên từ 20px đến 50px
                document.body.appendChild(icon);

                // Xóa biểu tượng với hiệu ứng mờ dần
                setTimeout(() => {
                    icon.style.animation = 'fadeOut 1s forwards'; // Thêm hiệu ứng mờ dần
                    setTimeout(() => {
                        icon.remove();
                    }, 1000); // Xóa sau 1 giây
                }, Math.random() * 2000); // Để các biểu tượng xuất hiện tại các thời điểm ngẫu nhiên
            }
        }

        // Hàm tạo bông hoa
        function createFlowers() {
            for (let i = 0; i < 5; i++) { // Tạo 5 bông hoa
                const flower = document.createElement('div');
                flower.className = 'flower';
                flower.innerText = "🌻"; // Biểu tượng hoa
                flower.style.left = `${Math.random() * 100}vw`; // Vị trí ngẫu nhiên từ trái sang phải
                flower.style.animationDelay = `${Math.random() * 2}s`; // Để hoa nở với độ trễ ngẫu nhiên
                document.body.appendChild(flower);

                // Xóa bông hoa sau một thời gian
                setTimeout(() => {
                    flower.remove();
                }, 1000); // Xóa sau 1 giây
            }
        }
    </script>

</body>
</html>

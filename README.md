<div class="content">
    <h1>BÁO CÁO KIỂM THỬ API</h1>
    <ol>
        <p><strong>Tên Dự Án:</strong> Test Collection of APIs</p>
        <p><strong>Ngày Kiểm Thử:</strong> 24/05/2024</p>
        <p><strong>Người Kiểm Thử:</strong> Giang Thành An</p>
        <p><strong>1. Mục Tiêu Kiểm Thử:</strong> Sử dụng Postman để kiểm thử một API thực tế</p>
        <p><strong>2. Môi Trường Kiểm Thử:</strong> Postman.</p>
        <p><strong>3. Phương Pháp Kiểm Thử:</strong> Kiểm thử tự động và thủ công trên phần mềm Postman.</p>
        4.
         <strong>Kịch Bản Kiểm Thử Lần 1:</strong>
            <ul>
            <li><p>Tên Kịch Bản: Kiểm thử cơ bản của 1 URL</p></li>
            <li><p>Mục Đích: Test khả năng hoạt động của URL và phần mềm Postman</p></li>
            <li><p>Phương Thức HTTP (GET/POST/PUT/DELETE): GET</p></li>
            <li><p>URL: https://random-data-api.com/api/v2/</p></li>
            <li><p>Tham Số: users?size=2&is_xml=true</p></li>
            <li><p>Kết Quả Mong Đợi: Gửi yêu cầu thành công</p></li>
            <li><p>Kết Quả Thực Tế: Đã gửi yêu cầu thành công</p></li>
            <li><p>Trạng Thái: Thành công</p></li>
            <li><p>Kết quả sau khi kiểm thử:</p></li>
            <img width="468" alt="image" src="https://github.com/gtaAsian/New-Collection-of-APIs/assets/170786444/c340d30f-fea5-4f45-b752-369a1f066f80">
            <li><p>Kết quả kiểm thử chi tiết:</p></li>
            </ul>
    
    [
        {  
        
            "id": 9209,
            "uid": "61b0ecef-a169-49c1-9b7e-616aebe82641",
            "password": "zWosu2p6UN",
            "first_name": "Davis",
            "last_name": "Hand",
            "username": "davis.hand",
            "email": "davis.hand@email.com",
            "avatar": "https://robohash.org/corruptiutrepudiandae.png?size=300x300&set=set1",
            "gender": "Genderfluid",
            "phone_number": "+223 522.344.8113",
            "social_insurance_number": "625916069",
            "date_of_birth": "1978-03-23",
            "employment": {
                "title": "Sales Consultant",
                "key_skill": "Problem solving"
            },
            "address": {
                "city": "Port Sid",
                "street_name": "Shizuko Unions",
                "street_address": "7042 Mei Union",
                "zip_code": "56023-6796",
                "state": "Texas",
                "country": "United States",
                "coordinates": {
                    "lat": 29.124815080601806,
                    "lng": -52.01789697476312
                }
            },
            "credit_card": {
                "cc_number": "6771-8982-4885-7139"
            },
            "subscription": {
                "plan": "Premium",
                "status": "Active",
                "payment_method": "Money transfer",
                "term": "Monthly"
            }
        },
        {
            "id": 4506,
            "uid": "1f8ef347-e420-4e50-8b66-8cf92ab6ad74",
            "password": "RQpDo89cFw",
            "first_name": "Trent",
            "last_name": "Quitzon",
            "username": "trent.quitzon",
            "email": "trent.quitzon@email.com",
            "avatar": "https://robohash.org/quibusdamautquisquam.png?size=300x300&set=set1",
            "gender": "Genderqueer",
            "phone_number": "+675 (698) 414-6258 x469",
            "social_insurance_number": "193053717",
            "date_of_birth": "1999-03-10",
            "employment": {
                "title": "Legal Administrator",
                "key_skill": "Leadership"
            },
            "address": {
                "city": "Schroederchester",
                "street_name": "Macejkovic Via",
                "street_address": "5634 Tyron Ferry",
                "zip_code": "75541",
                "state": "Alabama",
                "country": "United States",
                "coordinates": {
                    "lat": 22.21205024489973,
                    "lng": 139.04500158922622
                }
            },
            "credit_card": {
                "cc_number": "4409687671791"
            },
            "subscription": {
                "plan": "Starter",
                "status": "Pending",
                "payment_method": "Apple Pay",
                "term": "Full subscription"
            }
        }
    ]
<div>    
    <strong>Kịch Bản Kiểm Thử Lần 2:</strong>
            <ul>
            <li><p>Tên Kịch Bản: Kiểm thử cơ bản của một URL với một tham số</p></li>
            <li><p>Mục Đích: Test khả năng hoạt động của URL và phần mềm Postman</p></li>
            <li><p>Phương Thức HTTP (GET/POST/PUT/DELETE): GET</p></li>
            <li><p>URL: https://random-data-api.com/api/v2/</p></li>
            <li><p>Tham Số: beerType=light</p></li>
            <li><p>Kết Quả Mong Đợi: Gửi yêu cầu thành công</p></li>
            <li><p>Kết Quả Thực Tế: Gửi yêu cầu thất bại</p></li>
            <li><p>Trạng Thái: Không thành công</p></li>
            <li><p>Kết quả sau khi kiểm thử:</p></li>
            <img width="468" alt="image" src="https://github.com/gtaAsian/New-Collection-of-APIs/assets/170786444/47657a68-c2ce-4826-80db-863977b71169">
            <li><p>Kết quả kiểm thử chi tiết:</p></li>
            </ul>


    <!DOCTYPE html>
    <html>
    
    <head>
    
        <title>The page you were looking for doesn't exist (404)</title>
        <meta name="viewport" content="width=device-width,initial-scale=1">
        <style>
            .rails-default-error-page {
                background-color: #EFEFEF;
                color: #2E2F30;
                text-align: center;
                font-family: arial, sans-serif;
                margin: 0;
            }
            
            .rails-default-error-page div.dialog {
                width: 95%;
                max-width: 33em;
                margin: 4em auto 0;
            }
    
            .rails-default-error-page div.dialog>div {
                border: 1px solid #CCC;
                border-right-color: #999;
                border-left-color: #999;
                border-bottom-color: #BBB;
                border-top: #B00100 solid 4px;
                border-top-left-radius: 9px;
                border-top-right-radius: 9px;
                background-color: white;
                padding: 7px 12% 0;
                box-shadow: 0 3px 8px rgba(50, 50, 50, 0.17);
            }
    
            .rails-default-error-page h1 {
                font-size: 100%;
                color: #730E15;
                line-height: 1.5em;
            }
    
            .rails-default-error-page div.dialog>p {
                margin: 0 0 1em;
                padding: 1em;
                background-color: #F7F7F7;
                border: 1px solid #CCC;
                border-right-color: #999;
                border-left-color: #999;
                border-bottom-color: #999;
                border-bottom-left-radius: 4px;
                border-bottom-right-radius: 4px;
                border-top-color: #DADADA;
                color: #666;
                box-shadow: 0 3px 8px rgba(50, 50, 50, 0.17);
            }
        </style>
    </head>
    <body class="rails-default-error-page">
        <!-- This file lives in public/404.html -->
        <div class="dialog">
            <div>
                <h1>The page you were looking for doesn't exist.</h1>
                <p>You may have mistyped the address or the page may have moved.</p>
            </div>
            <p>If you are the application owner check the logs for more information.</p>
        </div>
    </body>

    </html>
<div>
    <strong>Kịch Bản Kiểm Thử Lần 1:</strong>
            <ul>
            <li><p>Tên Kịch Bản: Kiểm thử cơ bản của 1 URL với một tham số truyền vào</p></li>
            <li><p>Mục Đích: Test khả năng hoạt động của URL và phần mềm Postman</p></li>
            <li><p>Phương Thức HTTP (GET/POST/PUT/DELETE): GET</p></li>
            <li><p>URL: https://random-data-api.com/api/v2/</p></li>
            <li><p>Tham Số: beerType=light</p></li>
            <li><p>Kết Quả Mong Đợi: Gửi yêu cầu thành công</p></li>
            <li><p>Kết Quả Thực Tế: Đã gửi yêu cầu thành công</p></li>
            <li><p>Trạng Thái: Thành công</p></li>
            <li><p>Kết quả sau khi kiểm thử:</p></li>
            <img width="468" alt="image" src="https://github.com/gtaAsian/New-Collection-of-APIs/assets/170786444/4704b95c-115c-4e24-aa8a-2aeee5339fba">
            <li><p>Kết quả kiểm thử chi tiết:</p></li>
            </ul>
</div>

        {
            "id": 4908,
            "uid": "16d508f9-8757-491d-b8c9-4b980932f637",
            "brand": "Leffe",
            "name": "Sapporo Premium",
            "style": "Strong Ale",
            "hop": "Newport",
            "yeast": "1098 - British Ale",
            "malts": "Roasted barley",
            "ibu": "82 IBU",
            "alcohol": "2.1%",
            "blg": "12.8°Blg"
        }
        
<p><strong>5. Kết Quả Kiểm Thử:</strong> Tóm tắt kết quả kiểm thử, bao gồm số lượng kịch bản kiểm thử đã chạy, số lượng thành công, số lượng thất bại, và tỷ lệ thành công.</p>
<ul>
<li><p>Số lượng kịch bản đã kiểm thử: 3</p></li>
<li><p>Số lần thành công: 2</p></li>
<li><p>Số lần thất bại: 1</p></li>
<li><p>Tỉ lệ thành công: 75%</p></li>
</ul>
<p><strong>6. Phát Hiện Lỗi:</strong>  Chi tiết về lỗi, bao gồm:</p>
<ul>
<li><p>ID Lỗi: 404 Not Found</p></li>
<li><p>Mô Tả Lỗi: Trang bạn đang tìm kiếm không tồn tại (404)</p></li>
<li><p>Mức Độ Ảnh Hưởng: Không</p></li>
<li><p>Ghi Chú/Đề Xuất: Sai URL và tham số</p></li>
</ul>

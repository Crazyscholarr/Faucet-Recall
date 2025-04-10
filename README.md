# Faucet-Recall
# Faucet-Recall

! Warning: You should use a separate proxy for the wallet, if there are too many duplicates, you will not be able to send requests
# Faucet-Recall
# Faucet-Recall
Faucet Recall token support for the project with built-in features of capcha solution, retry if faucet failure, proxy integration
! Warning: You should use a separate proxy for the wallet, if there are too many duplicates, you will not be able to send requests
# Faucet Recall

## Introduction

**Faucet Recall** is an automated tool for requesting tokens from the Recall Network (testnet) faucet. The program uses Capsolver to solve Turnstile CAPTCHAs and supports proxies to send multiple requests from different wallets. It is designed to run continuously, automatically retry when errors occur, and can customize the log language (Vietnamese or English).

**Faucet Recall** is an automated tool for requesting tokens from the Recall Network (testnet) faucet. The program uses Capsolver to solve Turnstile CAPTCHAs and supports proxies to send multiple requests from different wallets. It is designed to run continuously, automatically retrying on errors, and allows log language customization (Vietnamese or English).

---

## Features

- **Faucet automation**: Send token requests to multiple wallets continuously.

- **CAPTCHA Solving**: Integrate Capsolver to bypass Turnstile CAPTCHA.

- **Proxy support**: Use proxy lists to avoid request limits.

- **Error handling**: Automatically retry when encountering errors such as `429 Too Many Requests`, `502 Bad Gateway`, or `Sequence Mismatch`.

- **Detailed log**: Display logs with timestamps, wallet status, and transaction information (supports Vietnamese and English).

- **Customization**: Easily configure via `.env` file.

- **Faucet automation**: Continuously sends token requests for multiple wallets.
- **CAPTCHA solving**: Integrates Capsolver to bypass Turnstile CAPTCHA.
- **Proxy support**: Uses a proxy list to avoid request limits.
- **Error handling**: Automatically retries on errors like `429 Too Many Requests`, `502 Bad Gateway`, or `Sequence Mismatch`.
- **Detailed logging**: Displays logs with timestamps, wallet status, and transaction information (supports Vietnamese and English).
- **Customizable**: Easily configured via `.env` file.

---

## Requirements

- **Node.js**: Version 16.x or higher.
- **Capsolver API Key**: Register at [Capsolver](https://www.capsolver.com/) to get the key.
- **Proxy**: Proxy list (optional, but recommended to avoid rate limit).

- **Node.js**: Version 16.x or higher.
- **Capsolver API Key**: Register at [Capsolver](https://www.capsolver.com/) to get a key.
- **Proxies**: Proxy list (optional, but recommended to avoid rate limits).

---

## Installation and Usage Instructions (Installation and Usage)

### 1. Clone repository
```bash
git clone git@github.com:Crazyscholarr/Faucet-Recall.git
cd Faucet-Recall
```
###2. Install dependencies
npm install
3. Prepare configuration file
Create a .env file in the root directory with the following content:
plaintext
```bash
CAPTCHA_SERVICE=capsolver
CAPSOLVER_KEY=<your_capsolver_api_key>
LANGUAGE=vi # or 'en' for English
```
Create a data/ directory and add two files:
data/private_keys.txt: List of wallet private keys, one per line.
```bash

0xabc123...
0xdef456...
```
data/proxies.txt: List of proxies (format http://username:password@host:port), one per line.
text

http://user1:pass1@123.456.789.012:8080
http://user2:pass2@987.654.321.098:8080
4. Run the program
```bash
node faucetRecall.js
```
# Faucet Recall


## Giới thiệu (Introduction)

**Faucet Recall** là một công cụ tự động để yêu cầu token từ faucet của Recall Network (testnet). Chương trình sử dụng Capsolver để giải CAPTCHA Turnstile và hỗ trợ proxy để gửi nhiều yêu cầu từ các ví khác nhau. Nó được thiết kế để chạy liên tục, tự động thử lại khi gặp lỗi, và có thể tùy chỉnh ngôn ngữ log (Tiếng Việt hoặc Tiếng Anh).

**Faucet Recall** is an automated tool for requesting tokens from the Recall Network (testnet) faucet. The program uses Capsolver to solve Turnstile CAPTCHAs and supports proxies to send multiple requests from different wallets. It is designed to run continuously, automatically retrying on errors, and allows log language customization (Vietnamese or English).

---

## Tính năng (Features)

- **Tự động hóa faucet**: Gửi yêu cầu token cho nhiều ví liên tục.
- **Giải CAPTCHA**: Tích hợp Capsolver để vượt qua Turnstile CAPTCHA.
- **Hỗ trợ proxy**: Sử dụng danh sách proxy để tránh giới hạn yêu cầu.
- **Xử lý lỗi**: Tự động thử lại khi gặp lỗi như `429 Too Many Requests`, `502 Bad Gateway`, hoặc `Sequence Mismatch`.
- **Log chi tiết**: Hiển thị log với timestamp, trạng thái ví, và thông tin giao dịch (hỗ trợ Tiếng Việt và Tiếng Anh).
- **Tùy chỉnh**: Dễ dàng cấu hình thông qua file `.env`.

- **Faucet automation**: Continuously sends token requests for multiple wallets.
- **CAPTCHA solving**: Integrates Capsolver to bypass Turnstile CAPTCHA.
- **Proxy support**: Uses a proxy list to avoid request limits.
- **Error handling**: Automatically retries on errors like `429 Too Many Requests`, `502 Bad Gateway`, or `Sequence Mismatch`.
- **Detailed logging**: Displays logs with timestamps, wallet status, and transaction info (supports Vietnamese and English).
- **Customizable**: Easily configured via `.env` file.

---

## Yêu cầu (Requirements)

- **Node.js**: Phiên bản 16.x hoặc cao hơn.
- **Capsolver API Key**: Đăng ký tại [Capsolver](https://www.capsolver.com/) để lấy key.
- **Proxy**: Danh sách proxy (tùy chọn, nhưng khuyến nghị để tránh rate limit).

- **Node.js**: Version 16.x or higher.
- **Capsolver API Key**: Register at [Capsolver](https://www.capsolver.com/) to get a key.
- **Proxies**: Proxy list (optional, but recommended to avoid rate limits).

---

## Hướng dẫn cài đặt và sử dụng (Installation and Usage)

### 1. Clone repository
```bash
git clone git@github.com:Crazyscholarr/Faucet-Recall.git
cd Faucet-Recall
```
###2. Cài đặt dependencies
  npm install 
3. Chuẩn bị file cấu hình
Tạo file .env trong thư mục gốc với nội dung sau:
plaintext

CAPTCHA_SERVICE=capsolver
CAPSOLVER_KEY=<your_capsolver_api_key>
LANGUAGE=vi  # hoặc 'en' để dùng Tiếng Anh
Tạo thư mục data/ và thêm hai file:
data/private_keys.txt: Danh sách private keys của ví, mỗi key trên một dòng.
text

0xabc123...
0xdef456...

data/proxies.txt: Danh sách proxy (định dạng http://username:password@host:port), mỗi proxy trên một dòng.
text

http://user1:pass1@123.456.789.012:8080
http://user2:pass2@987.654.321.098:8080
4. Chạy chương trình
```bash
node faucetRecall.js
```

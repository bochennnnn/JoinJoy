# JoinJoy

> JoinJoy 是一個活動平台，使用者可以報名參與活動、發起活動以及發起討論文章，透過共同平台讓有相同興趣的各位有更多相遇的機會。

> 本來專案是放在 Azure 雲端，後來自行研究把整個專案用 Docker 打包及部署到 Google Cloud Platform（GCP），也有 namecheap 購買域名，目前尚有一些 bug，但會員登入/註冊/忘記密碼（包括Google登入）的功能都正常執行，可以點選[連結](https://joinjoybc.online/)到我們網站瀏覽。

- [線上觀看連結](https://joinjoybc.online/)

![Untitled](Img_md/Untitled.png)

## 功能

> 我開發功能為，會員的登入/註冊/忘記密碼，是以 Spring Security 框架下開發，除了會員註冊可以選擇原本網站的註冊，也可以選擇第三方 Google 帳號登入/註冊，並在網站的設有帳號認證權限管制；且結合 Redis 來存取信箱OTP驗證碼的功能，加上驗證碼的時效以及次數限制。
> 

測試帳號密碼

```bash
帳號： ispan3939889@gmail.com
密碼： password2

```

## 畫面

> 首頁
> 

![screencapture-localhost-8081-2024-05-13-15_56_27.png](Img_md/screencapture-localhost-8081-2024-05-13-15_56_27.png)

> 登入/註冊/忘記密碼
> 

![Untitled](Img_md/Untitled%201.png)

![Untitled](Img_md/Untitled%202.png)

![Untitled](Img_md/Untitled%203.png)

> 第三方登入（Google）
> 

![截圖 2024-05-13 下午3.59.43.png](Img_md/%25E6%2588%25AA%25E5%259C%2596_2024-05-13_%25E4%25B8%258B%25E5%258D%25883.59.43.png)

## 專案技術

> 使用的 Java 版本為 17；Spring Boot 版本為 3.2.3；建置工具使用 Maven。
> 
- 前端
    - Vue v3.4.21
    - Axios v1.6.8
    - Bootstrap v5.2.3
    - ...
- 後端
    - JDK 17
    - Spring Boot v3.2.3
    - Spring Security
    - Hibernate
    - Spring Mail
    - ...

## 資料庫

- MS SQL
- Redis

## 第三方服務

- Google OAuth
- ...

## 環境變數說明

### 我所使用的

- **發送方帳號 (`spring.mail.username`):**
您的郵件帳號，用於發送郵件。
- **發送方密碼 (`spring.mail.password`):**
您的郵件帳號對應的密碼或授權碼，用於驗證身份以發送郵件。
- **Google OAuth2 客戶端 ID (`spring.security.oauth2.client.registration.google.client-id`):**
如果您的應用使用了 Google OAuth2 進行身份驗證，則需要填入您的 Google OAuth2 客戶端 ID。
- **Google OAuth2 客戶端密鑰 (`spring.security.oauth2.client.registration.google.client-secret`):**
如果您的應用使用了 Google OAuth2 進行身份驗證，則需要填入您的 Google OAuth2 客戶端密鑰。

### 其他組員使用

- **GCP 專案 ID (`spring.cloud.gcp.project-id`):**
如果您的應用使用了 Google Cloud Storage，則需要填入您的 GCP 專案 ID。
- **GCP 憑證位置 (`spring.cloud.gcp.credentials.location`):**
如果您的應用使用了 Google Cloud Storage，則需要填入 GCP 憑證文件的位置。
- **AWS S3 Bucket 名稱 (`aws.s3.bucket-name`):**
如果您的應用使用了 AWS S3，則需要填入您的 AWS S3 Bucket 名稱。
- **AWS Region (`aws.s3.region`):**
如果您的應用使用了 AWS S3，則需要填入您的 AWS Region。
- **AWS Access Key ID (`aws.access-key-id`):**
如果您的應用使用了 AWS，則需要填入您的 AWS Access Key ID。
- **AWS Secret Access Key (`aws.secret-access-key`):**
如果您的應用使用了 AWS，則需要填入您的 AWS Secret Access Key。

## 聯絡作者

你可以透過以下方式與我聯絡

- [LinkedIn](https://www.linkedin.com/in/bo-chen-lin-a0b429224/)
- [104人力銀行](https://pda.104.com.tw/profile/share/8sdVprJszq4NlKZQujkViUZQMwnAjWRn)
- ...


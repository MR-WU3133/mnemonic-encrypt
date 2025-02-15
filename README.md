# Mnemonic Encryption Tool

**Author: MR.WU**  
**Official Website: [mnemonic-encryption-tool.mystrikingly.com](https://mnemonic-encryption-tool.mystrikingly.com)**

## Introduction
Mnemonic Encryption Tool is an open-source encryption tool designed to enhance the security of mnemonic phrases through multi-layered protection. 
It converts mnemonic phrases into highly secure formats using customizable encryption parameters, making it ideal for safeguarding sensitive data stored physically (e.g., on paper or metal plates).


## Features

- **Mnemonic to Numeric Conversion**: Converts mnemonic phrases into numerical format.
- **Shift Encryption**: Uses a shift value (0-25) for letter transformation.
- **Number Splitting**: Automatically converts input numbers into two-digit format.
- **Sequential Value Insertion**: Allows users to insert 1-6 sequential values.
- **Secondary Encryption**: Adds an extra layer of encryption with six additional numbers.
- **Letter Encryption Option**: Converts the final encrypted result into shifted encrypted letters.

### Encryption Process
##  Mnemonic to Numbers
Convert each mnemonic word into its corresponding five-digit number based on the BIP-39 standard.
(Example: apple → 04081)

##  Number Segmentation
Split the long numerical string into two-digit groups.
(Example: 04081 → 00-04-00-08-01)

##  Letter Shift Encryption
The user sets a custom shift value (0-25) to offset numbers into letters.
(Example: With a shift of 1, 0 → C)

##  Sequential Value Insertion
Insert a sequence value at a predefined position in the segmented numbers.
(Example: Insert position 15 at the third number → apple → 04081 → 00-04-15-00-08-01)

##  Secondary Encryption
Add six custom encryption values (0-9) to further secure the sequence.
(Example: Add 123456 → 00-04-15-00-08-01 → 01 06 18 04 13 07)

##  Letter Encoding
Optionally, convert the final numeric result into shifted letters.
(Example: apple → 04081 → 00-04-00-15-08-01 → 01 06 18 04 13 07 → CHTFOI)

## Installation and Usage

### Download

1. Visit [GitHub Releases](https://github.com/MR-WU3133/mnemonic-encrypt) to download the latest version of `mnemonic_encrypt.exe`.
2. To verify file integrity, download the corresponding GPG signature file (`mnemonic_encrypt_MR.WU.sig`).

### Execution

Windows users can run `mnemonic_encrypt.exe` directly. Linux and macOS users can use the Python version (if available).

### Signature Verification

To verify the integrity of the EXE file:

```sh
gpg --import public_key.asc
gpg --verify mnemonic_encrypt_MR.WU.sig mnemonic_encrypt.exe
```

If you see `Good signature from "MR.WU"`, it means the file has not been tampered with.

## Open Source and Contributions

This project is licensed under **MIT License**, allowing free modification and use, but the following rules must be followed:

- **Original Author Attribution**: The original author, MR.WU, must be credited, and the official website [mnemonic-encryption-tool.mystrikingly.com](https://mnemonic-encryption-tool.mystrikingly.com) must be displayed in the program.
- **Donation Address Requirement**: Any derivative work must include at least one of the following donation addresses within the program:
  - **ADA**: addr1q8jjupw3y7dgmektm78f6f3nm56cksgrvtamhydqf3ryjgs0c3z3eppjvghdrhtq6swhmgv7gfuax0ygnzkzlpk3qqcsy0jdgj
  - **ETH(ARB)**: 0xBFF3B7631A32f0439b3f1bFad8c1E0066aB7109c
  - **BTC**: bc1p4m8636d5hzhkzurrxss39crx8p2zl08gjkpqy544wmyq8g8gh4xstvfhzs
  - **BSC**: 0xBFF3B7631A32f0439b3f1bFad8c1E0066aB7109c
  - **DOGE**: DEUcv2wRNoZbG7huqAfEXZjqBdUVpuWcZ3

For contributions or issues, please submit a Pull Request or Issue on GitHub.

## Contact

For any inquiries, please visit [Official Website](https://mnemonic-encryption-tool.mystrikingly.com) or contact MR.WU.

- **Instagram**: [han313_c](https://www.instagram.com/han313_c)
- **Telegram Official Channel**: [Encryption Tool WU](https://t.me/encryptiontoolWU)

---
## Warning
You must securely store the following information:

Shift Value
Sequence Insertion Positions
Secondary Encryption Values
Losing any of these parameters will result in permanent inability to decrypt!

Recommended 3-2-1 Backup Strategy:
- ✅ 3 copies of the backup
- ✅ 2 different storage media
- ✅ 1 copy stored in a remote location
-
Make sure to back up your shift values and sequence values. If lost, decryption will be impossible!


---

# Mnemonic Encryption Tool-中文說明

**作者：MR.WU**  
**官方網站：[mnemonic-encryption-tool.mystrikingly.com](https://mnemonic-encryption-tool.mystrikingly.com)**

## 介紹

Mnemonic Encryption Tool 是一款開源的助記詞加密工具，專為保護區塊鏈助記詞設計。
透過多層加密演算法，將助記詞轉換為高度安全的數字/字母組合，有效防止實體儲存媒體（紙張、金屬板）被盜時的資訊外洩。

## 功能

- **助記詞數字轉換**：將助記詞轉換為數值格式。
- **偏移加密**：使用 0~25 的偏移值進行字母轉換。
- **數字拆分**：將輸入的數字自動轉換為 2 位數格式。
- **順序值插入**：允許使用者插入 1~6 位順序值。
- **二次加密**：使用額外 6 位數對加密數據進行進一步保護。
- **英文字母加密選項**：可選擇將最終加密結果轉換為含加密後並偏移的英文字母。

### 加密流程

## 助記詞轉數字
**根據標準BIP-39詞表，將每個助記詞轉換為對應的五位數（例：apple → 04081）**

## 數位分割
**將長數字串分割為兩位數組合（例：04081 → 00-04-00-08-01）**

## 位移字母加密
**使用者自訂位移值（0-25），對數字進行字母偏移加密（例：位移1時，0 → C ）**

## 序列值插入
**在分割後的數字間插入順序值（例：第三位數插入第15順序的順序值 → apple → 04081 → 00-04-15-00-08-01）**

## 二次加密
**新增6位0~9數字自訂加密值（例：新增123456 →  00-04-15-00-08-01 → 01 06 18 04 13 07 ）**

## 字母編碼
**可選將最終數字轉換為偏移後字母（apple → 04081 → 00-04-00-15-08-01 → 01 06 18 04 13 07 → CHTFOI）**

## 安裝與使用

### 下載

1. 下載最新版本的[GitHub Releases](https://github.com/MR-WU3133/mnemonic-encrypt) `mnemonic_encrypt.exe`。
2. 若需要驗證文件完整性，請下載對應的 GPG 簽名文件 (`mnemonic_encrypt_MR.WU.sig`)。

### 執行方式

Windows 用戶可以直接執行 `mnemonic_encrypt.exe`，Linux 和 macOS 用戶可以使用 Python 版本（若提供）。

### 驗證簽名

若要驗證 EXE 檔案的完整性：

```sh
 gpg --import public_key.asc
 gpg --verify mnemonic_encrypt_MR.WU.sig mnemonic_encrypt.exe
```

若顯示 `Good signature from "MR.WU"`，表示該程式未被修改。

## 開源與貢獻

本專案基於 **MIT 授權**，允許自由修改與使用，但須遵守以下規則：

- **標註原作者 MR.WU**，並在程式內顯示官方網站：[mnemonic-encryption-tool.mystrikingly.com](https://mnemonic-encryption-tool.mystrikingly.com)
- **捐款地址要求**：二創者需在程式內包含以下任一捐款地址：
  - **ADA**: addr1q8jjupw3y7dgmektm78f6f3nm56cksgrvtamhydqf3ryjgs0c3z3eppjvghdrhtq6swhmgv7gfuax0ygnzkzlpk3qqcsy0jdgj
  - **ETH(ARB)**: 0xBFF3B7631A32f0439b3f1bFad8c1E0066aB7109c
  - **BTC**: bc1p4m8636d5hzhkzurrxss39crx8p2zl08gjkpqy544wmyq8g8gh4xstvfhzs
  - **BSC**: 0xBFF3B7631A32f0439b3f1bFad8c1E0066aB7109c
  - **DOGE**: DEUcv2wRNoZbG7huqAfEXZjqBdUVpuWcZ3

如需貢獻代碼或提交問題，請在 GitHub 上提交 Pull Request 或 Issue。

## 聯繫方式

若有任何問題，請訪問 [官方網站](https://mnemonic-encryption-tool.mystrikingly.com) 或聯繫 MR.WU。

- **Instagram**：[han313_c](https://www.instagram.com/han313_c)
- **Telegram 官方頻道**：[Encryption Tool WU](https://t.me/encryptiontoolWU)

## 更新日誌
---

## 警告
**請必須妥善保存以下資訊：
1. 位移值
2. 插入順序值位置
3. 二次加密值

- 遺失任何參數將導致永久無法解密！
- 建議採用3-2-1備份原則：
- 3份備份
- 2種介質
- 1份異地存儲
-
**請確保備份您的偏移值與順序值，遺失後將無法解密！**




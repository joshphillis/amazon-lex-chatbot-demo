# amazon-lex-chatbot-demo

# 🏨 HotelBookingBot — Voice & Text Chatbot Powered by Amazon Lex V2

## Overview  
**HotelBookingBot** is a conversational AI chatbot built using **Amazon Lex V2**. It enables users to seamlessly book hotel accommodations via voice or text by capturing key details such as location, check-in and check-out dates, and confirmation preferences. Powered by natural language understanding and AWS cloud services, this project demonstrates chatbot design principles for real-world use cases.

## 🔧 Technologies Used
- **Amazon Lex V2** – Natural language processing & dialogue flow management  
- **Amazon CloudWatch** – Logging for bot diagnostics and error tracking  
- **IAM Roles** – Granular permissions for secure service interaction  

## 🗣️ Bot Features
- **Descriptive Bot Builder** via Amazon Bedrock  
- Voice-enabled interaction using **Danielle (English-US)**  
- Slot handling for:
  - `Location` (AMAZON.City)
  - `CheckInDate` (AMAZON.Date)
  - `CheckOutDate` (AMAZON.Date)
- Confirmation flow: "Can I go ahead and book this hotel?"  
- Closing response: “Thanks! I have booked your room in _{Location}_ from _{CheckInDate}_ to _{CheckOutDate}_.”

## 📈 Key Lessons & Troubleshooting Highlights
- Case sensitivity of slot names impacts closing response fulfillment  
- Fixed `sessionId` key error by disabling default Lambda invocation under initial response  
- Implemented proper build sequence for the draft version and tested with live utterance flow

## 🚀 How to Use
1. Log into your AWS Console  
2. Navigate to **Amazon Lex V2** service  
3. Create or import the bot configuration  
4. Test utterances in the test workbench  
5. Monitor logs and performance via **CloudWatch Metrics** and **Analytics Dashboard**
---

## 🔗 Useful Links
- [Amazon Lex V2 Documentation](https://docs.aws.amazon.com/lexv2/)
- [AWS IAM Role Setup](https://docs.aws.amazon.com/IAM/latest/UserGuide/)
- [Amazon Bedrock Overview](https://docs.aws.amazon.com/bedrock/)
- [Amazon CloudWatch Logs](https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/)



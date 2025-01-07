AWS SNS Notification System

This project demonstrates how to use **Amazon Simple Notification Service (SNS)** to send real-time email and SMS notifications for critical alerts.


Project Overview

The system consists of:  
1. **SNS Topic**: Used to manage and broadcast notifications to multiple subscribers.  
2. **Subscribers**: Email and SMS recipients who receive notifications.  
3. **Automation**: An optional AWS Lambda function to trigger notifications automatically.


## **Features**

- Send notifications via email and SMS.  
- Automate alerts for system errors or critical updates.  
- Real-time message delivery.  
- Easily scalable and integrates with other AWS services.  



## **Setup Instructions**

### **1. Create SNS Topic**
1. Log in to your AWS Management Console.  
2. Navigate to the **SNS** service.  
3. Create a new SNS topic named `CriticalAlerts`.  

### **2. Add Subscriptions**
- Add **Email** subscriptions for email notifications.  
- Add **SMS** subscriptions for phone alerts.  
- Confirm the email subscription by verifying the confirmation email sent by AWS.

### **3. Publish a Message**
1. Open your SNS topic in the console.  
2. Click `Publish message`.  
3. Enter a subject and message.  
4. Click `Publish`.  
5. Verify that all subscribers receive the notification.

### **4. Automate Alerts with AWS Lambda (Optional)**
- Deploy a Lambda function to trigger SNS notifications automatically.  
- Integrate with AWS CloudWatch Alarms, S3 Events, or other AWS services.



## **Project Files**

- `README.md`: Project documentation.  
- `lambda_function.py`: AWS Lambda function to publish messages to SNS.  

## **How to Test**

1. Publish test messages via the AWS console.  
2. Verify that email and SMS subscribers receive the notifications.  
3. For Lambda integration, trigger the function and confirm message delivery.



## **Future Enhancements**

- Add more subscription protocols like HTTP/HTTPS or mobile push.  
- Integrate with CloudWatch for error-based notifications.  
- Expand automation with triggers for various AWS events.





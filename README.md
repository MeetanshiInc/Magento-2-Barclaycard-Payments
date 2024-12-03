# **Magento 2 Barclaycard Payments Extension**

Efficient and secure payment processing is a cornerstone of successful eCommerce operations. Meetanshi's **Magento 2 Barclaycard Payments Extension** bridges the gap between businesses and their customers by offering a seamless, secure and versatile payment gateway powered by Barclaycard.

This extension ensures smooth payment experiences while adhering to the latest PCI compliance and security standards, making it an indispensable tool for Magento 2 store owners looking to streamline their payment process.

## **How It Works**

The **Magento 2 Barclaycard Payments Extension** integrates directly with your Magento 2 store. By connecting with Barclaycard, it facilitates secure transactions for credit cards, debit cards and other payment methods, using APIs that prioritize speed and accuracy.

Once installed and configured, customers can easily select Barclaycard as their payment option during checkout, ensuring a frictionless purchase journey. Store owners benefit from real-time transaction updates and detailed reports through the Magento backend.

## **Key Features**

* Supports all major credit and debit cards.  
* Direct Payment or Hosted Payment Page Options  
* CVC Verification and 3D Secure Enabled for Hosted Payments  
* Real-time payment processing with detailed logs.

## **Streamlined Payment Processing**

Enables seamless, redirect-free payment transactions, reducing cart abandonment with a faster and hassle-free checkout process.

## **Advanced Security**

Ensures robust data security with PCI DSS compliance, safeguarding sensitive customer information through advanced encryption protocols for every transaction.

## **Multi-Currency Support**

Supports multiple currencies for seamless international sales, with automatic price conversion based on real-time exchange rates.

## **Enhanced Customer Experience**

Provides a quick, intuitive checkout experience with the added convenience of securely saving payment details for future transactions.

## **Extension Installation**

To install the **Magento 2 Barclaycard Payments Extension**, follow these steps:

### **Step 1:** 

Unzip the folder and upload the extension to the root directory of your Magento 2 installation using FTP.

### **Step 2:** 

### Login to your SSH and run below commands step by step:

* php bin/magento setup:upgrade  
* For Magento version 2.0.x to 2.1.x \- php bin/magento setup:static-content:deploy  
* For Magento version 2.2.x & above \- php bin/magento setup:static-content:deploy –f  
* php bin/magento cache:flush 

**How to Configure Magento 2 Barclaycard Payments Extension**

### **Step 1: Barclaycard Account Signup and Login**

To integrate Barclaycard with Magento 2, start by signing up for a merchant account. Complete the registration form with the required details and submit it to successfully create your account with the Barclaycard Payment Gateway.

![Barclaycard Account Signup and Login](https://github.com/user-attachments/assets/076b18f2-ac38-4920-ba0f-2f04b607b1e4)

* **Enabled:**Toggle this option to "Yes" to enable the Barclaycard direct payment method  
* **Title:**Enter the title to display for this payment method on the frontend checkout page (e.g., Barclaycard ePDQ Direct Payment)  
* **3D Secure:** Choose "Enable" to activate 3D Secure for added transaction security.  
* **PSPID:** Enter your Payment Service Provider ID (PSPID) provided during registration with Barclaycard.  
* **User ID and Password:** Use the credentials (User ID and Password) assigned during your API user registration. These are essential for secure authentication.  
* **Alias:** If you have created an alias in the Barclaycard backend, enter it here for streamlined payment management.  
* **Hash Algorithm:** Select the same hash algorithm (e.g., SHA-512) that you configured in the Barclaycard backend for secure data integrity.  
* **SHA-In Passphrase:** Input the SHA-In passphrase configured in Barclaycard under "Configuration \-\> Technical Information \-\> Data and Origin.  
* **Sandbox Mode**: Set to "YES" to enable sandbox mode for testing the payment gateway.  
* **Order Prefix**: Specify a prefix for the orders processed through Barclaycard.  
* **Payment Action**: Choose the desired action for payment processing:  
* **Authorize**: Authorizes the payment and captures the amount after the invoice is generated.  
* **Authorize and Capture**: Authorizes the payment, captures the amount immediately and generates the invoice for the order.  
* **New Order Status**: Select the default status for newly placed orders.  
* **Credit Card Types**: Specify the credit card types that customers can use for payments.  
* **Payment from Applicable Countries**: Choose the countries where this payment method will be available.  
* **Enable Debug**: Set to "YES" to enable debug mode for troubleshooting and logging.  
* **Sort Order:** Enter the display order for this payment method on the frontend checkout page.

### **Sep 2: CHeck Barclaycard Direct Payment on the Frontend**

![CHeck Barclaycard Direct Payment on the Frontend](https://github.com/user-attachments/assets/d3469e59-ee37-485e-a72f-95ff892b7656)

After configuring the extension, the Barclaycard Direct Payment method becomes available on the frontend. Customers can add products to their cart and proceed to checkout, where they will see the Barclaycard payment option. By selecting it, entering their card details and confirming the payment, they can complete their order seamlessly.

### **Step 3: Payment Transaction Authentication**

![Payment Transaction Authentication](https://github.com/user-attachments/assets/6e0964af-89af-4c24-81ae-0d24a602d291)

When 3D Secure is enabled in the configuration, customers will need to authenticate their payment during checkout. The authentication process may vary depending on the card issuer and bank. Customers simply need to follow the provided authentication steps and submit the details to complete the payment successfully

### **Step 4: Payment Success on Barclaycard Hosted Payment Page**

![Payment Success on Barclaycard Hosted Payment Page](https://github.com/user-attachments/assets/2ffcb5db-a196-4fa2-81e5-f04c6c022c1e)

Upon successful payment, the Barclaycard hosted payment page displays a success message and seamlessly redirects customers back to the merchant's website.

### **Step 5: Barclaycard Payment Details in the My Account Section**

![Barclaycard Payment Details in the My Account Section](https://github.com/user-attachments/assets/7f6dfef3-aae4-43a0-8652-b8f95e3d5e04)

After placing an order, customers can view Barclaycard payment details, including payment type, card number, pay ID and transaction status, within the order view in the My Account section.

### **Step 6: Barclaycard Payment Details in Order View (Backend)**

![Barclaycard Payment Details in Order View](https://github.com/user-attachments/assets/63af0945-9654-49ee-a909-0a820f52ab35)

In addition to the My Account section, Barclaycard payment details are accessible in the backend under **Sales → Orders → Order View**.

### **Step 7: Barclaycard Payment Method for Backend Orders**

![Barclaycard Payment Method for Backend Orders](https://github.com/user-attachments/assets/931ba0a3-9012-44a4-8c98-ab2129c0d5af)

The Barclaycard payment method is fully functional for backend orders as well. Administrators can create a new order, select the Barclaycard payment option, enter the card details and submit the order to process the payment directly from the backend.

### **Step 8: Online Refund for Authorized Orders**

![Online Refund for Authorized Orders](https://github.com/user-attachments/assets/348e4e98-99b0-4cc0-be26-780537742a35)

For orders with "Authorize" selected under "Payment Action," invoices must be created manually. To do this, navigate to **Sales → Orders → Order View** and click **Submit Invoice** to generate the invoice for the order.

**Step 9: Online Refund for Barclaycard Authorized Orders**

![Online Refund for Barclaycard Authorized Orders](https://github.com/user-attachments/assets/db9ce598-b274-4039-b151-65c00e79d82c)

If "Authorize" is selected under the "Payment Action" setting, you can process online refunds for authorized orders by following these steps: Navigate to Sales → Orders → Order View → Invoice, click on Credit Memo and then select the Refund button to complete the online refund.

## Download our [Magento 2 Barclaycard Payments](https://meetanshi.com/magento-2-barclaycard-payments.html) Extension

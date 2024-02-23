

# Amazon Selenium WebDriver Script

This Selenium WebDriver script is designed to automate certain actions on the Amazon website, such as logging in, searching for a product, and initiating the purchase process. Please note the following information for successful execution.

## Prerequisites:

1. **WebDriver:**
   - Ensure you have the ChromeDriver executable downloaded and its path specified correctly.
   - Download ChromeDriver: [ChromeDriver Downloads](https://sites.google.com/chromium.org/driver/)

2. **Java:**
   - Make sure you have Java installed on your machine.
   - Download Java: [Java Downloads](https://www.oracle.com/java/technologies/javase-downloads.html)

## Execution Steps:

1. **Clone the Repository:**
   - Clone this repository to your local machine.

   ```bash
   git clone https://github.com/yourusername/your-repo.git
   ```

2. **Open Project in IDE:**
   - Open the project in your preferred Java IDE (Eclipse, IntelliJ, etc.).

3. **Update ChromeDriver Path:**
   - Open the `Test.java` file and ensure that the path to the ChromeDriver executable is correctly specified.

   ```java
   System.setProperty("webdriver.chrome.driver", "E:\\Drivers\\ChromeDriver\\chromedriver.exe");
   ```

4. **Update Login and Search Information:**
   - Update the email/phone, password, and item name in the script.

   ```java
   driver.findElement(By.id("ap_email")).sendKeys("enter_your_emailid_or_phonenumber_here");
   driver.findElement(By.id("ap_password")).sendKeys("enter_your_password_here");
   driver.findElement(By.id("twotabsearchtextbox")).sendKeys("enter_your_item_name_here");
   ```

5. **Run the Script:**
   - Run the `Test.java` file as a Java Application.

6. **Verify Execution:**
   - Monitor the browser as the script performs actions on the Amazon website.
   - Adjust implicit wait times and selectors as needed.

## Important Considerations:

- **CAPTCHA:**
  - The script may not handle CAPTCHA challenges. If CAPTCHA is encountered, manual intervention might be required.
  - Running the script in a controlled test environment is recommended.

- **Two-Factor Verification:**
  - The script might not work if two-factor verification is enabled for the Amazon account.

- **Selectors:**
  - Review and update the CSS selector for the first search result in the `Test.java` file based on the actual structure of the Amazon website.



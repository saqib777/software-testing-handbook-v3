# Testing Types

1. **Functional Testing**  
   Ensures the system works according to requirements.  
   Example: A shopping cart correctly adds and removes products.

   🔹 What is Functional Testing?

Functional testing is a type of software testing where we check if the system’s features (functions) behave as expected according to requirements or specifications.

In other words:
👉 Does the software do what it’s supposed to do?

We don’t care how it works internally (that’s white-box testing). Instead, we test the software like a user would.

🔹 Key Points

Focus: What the system does (not how).

Based on: Requirements, use cases, or business rules.

Done by: Testers (sometimes developers for unit testing).

Methods: Manual testing or automation.

Tools: Selenium, QTP, Postman (for APIs), etc.

🔹 Example

Imagine you’re testing an e-commerce website.

Requirement:
The shopping cart must let users:

Add a product.

Remove a product.

Update the quantity.

Functional Test Cases:

Add 1 product → ✅ Cart shows 1 item.

Add 2nd product → ✅ Cart shows 2 items.

Remove product → ✅ Cart updates correctly.

Update quantity from 1 → 3 → ✅ Total price updates.

If these expected outcomes happen → the function works.
If not → bug found.

🔹 Example in Real Life

Login Page: Enter valid username & password → user logs in.

Banking App: Transfer $100 → balance decreases by $100.

Search Engine: Enter a keyword → correct results displayed.

🔹 Why Functional Testing is Important

Ensures the product actually meets business needs.

Builds trust with stakeholders and users.

Helps catch critical bugs early.

⚡ In short:
Functional testing = Validating “What” the system does, by checking actual behavior against expected requirements.

3. **Non-Functional Testing**  
   Tests aspects like performance, usability, security.  
   Example: Checking if the website loads within 2 seconds under heavy traffic.

4. **Regression Testing**  
   Ensures new changes do not break old features.  
   Example: After adding a discount feature, verifying checkout still works.

5. **Smoke Testing**  
   Quick checks to confirm major functions are working.  
   Example: After deployment, verifying if login page loads successfully.

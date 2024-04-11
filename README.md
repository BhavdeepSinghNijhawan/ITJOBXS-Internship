# ITJOBXS

## TASKS

- Enhancing user verification and authentication processes.
- Addressing issues related to fake accounts and spam postings on the website.
- Design and development of a fully responsive web page for a specific section of itjobxs.com.
- User verification/authentication and addressed engineering challenges associated with detecting and removing fake bots and posts.
- Integrate Google reCAPTCHA with the website to provide an additional layer of protection against bots.

## PROBLEM

One issue that emerged on the itjobxs.com website was the proliferation of fake accounts, leading to vulgar content and rapidly filling up the database. Bots were registering multiple fake accounts and using the platform to post advertisements for various websites, disrupting the user experience.

## SOLUTION

### TEMPORARY SOLUTION

- Implemented a temporary solution by identifying email domains commonly associated with fake accounts (e.g., not gmail.com, hotmail.com, yahoo.com).
- Developed a PHP script to periodically delete users with email domains outside the specified list from the database.

### PERMANENT SOLUTION

- Introduced a check condition in the PHP registration process to reject users with email domains not on the approved list.
- Identified the need for a more robust solution to avoid false positives and ensure genuine users are not inadvertently blocked.

### FINAL SOLUTION

- Developed a comprehensive solution by creating a hashmap in PHP containing the top 100 valid domain names similar to Gmail.com.
- Modified the registration process to validate email domains against the hashmap, rejecting those not present.
- Integrated Google reCAPTCHA into the website's registration form to further enhance security and prevent bot registrations.

### OUTCOME

- By implementing the final solution, we significantly reduced the presence of fake accounts on itjobxs.com.
- The integration of Google reCAPTCHA enhanced the website's security and ensured that only genuine users could register, improving the overall user experience.

## TECHNICAL STACKS

- HTML
- CSS
- JavaScript
- Bootstrap
- PHP
- MySQL

## CONTRIBUTOR

- [Bhavdeep Singh Nijhawan](https://www.linkedin.com/in/bhavdeep-singh-nijhawan-739634280)

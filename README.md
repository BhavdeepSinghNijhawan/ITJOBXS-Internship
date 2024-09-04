<h1 align="center">ITJOBXS</h1>

## TASKS

- Enhancing **user verification and authentication** processes.
- Addressing issues related to **fake accounts** and **spam postings** on the website.
- Design and development of a fully responsive web page for a **specific section** of **`itjobxs.com`**.
- **User verification/authentication** and addressed engineering challenges associated with detecting and removing **fake bots** and **posts**.
- Integrate **Google reCAPTCHA** with the website to provide an additional layer of protection against bots.

## PROBLEM

One issue that emerged on the **`itjobxs.com`** website was the proliferation of fake accounts, leading to vulgar content and rapidly filling up the database. Bots were registering multiple fake accounts and using the platform to post advertisements for various websites, disrupting the user experience.

<div align="center">
  <img src="https://github.com/BhavdeepSinghNijhawan/ITJOBXS-Internship/assets/143419096/000ccaf9-ed38-4b14-b009-aa873f2cac0a" alt="Image">
</div>

## SOLUTION

### TEMPORARY SOLUTION

- Implemented a temporary solution by identifying email domains commonly associated with fake accounts (e.g., not gmail.com, hotmail.com, yahoo.com).
- Developed a **PHP script** to periodically delete users with email domains outside the specified list from the database.

### PERMANENT SOLUTION

- Introduced a check condition in the **PHP registration process** to reject users with email domains not on the **approved list**.
- Identified the need for a **more robust solution** to avoid **false positives** and ensure **genuine users are not inadvertently blocked**.

### FINAL SOLUTION

- Developed a comprehensive solution by **creating a hashmap in PHP** containing the **top 100 valid domain names similar to `gmail.com`**.
- Modified the registration process to validate email domains against the hashmap, rejecting those not present.
- Integrated **Google reCAPTCHA** into the **website's registration form** to further **enhance security** and **prevent bot registrations**.

```
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous">
```

<div align="center">
  <img src="https://github.com/BhavdeepSinghNijhawan/ITJOBXS-Internship/assets/143419096/fa64e06f-f8e8-4f15-9e5c-e1fb4d2fce3d" alt="Image">
</div>

<div align="center">
  <img src="https://github.com/BhavdeepSinghNijhawan/ITJOBXS-Internship/assets/143419096/95c5a1aa-4052-4b03-a701-56ecdeed3c71" alt="Image">
</div>

#### FORM

```
<form>
  <div class="mb-3">
    <label for="exampleInputEmail1" class="form-label">Email address</label>
    <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp">
    <div id="emailHelp" class="form-text">We'll never share your email with anyone else.</div>
  </div>
  <div class="mb-3">
    <label for="exampleInputPassword1" class="form-label">Password</label>
    <input type="password" class="form-control" id="exampleInputPassword1">
  </div>
  <div class="mb-3 form-check">
    <input type="checkbox" class="form-check-input" id="exampleCheck1">
    <label class="form-check-label" for="exampleCheck1">Check me out</label>
  </div>
  <button type="submit" class="btn btn-primary">Submit</button>
</form>
```

### OUTCOME

- By implementing the final solution, the presence of fake accounts on **`itjobxs.com`** reduced significantly.
- The integration of **Google reCAPTCHA** enhanced the website's security and ensured that only **genuine users could register*8, **improving the overall user experience**.

## TECHNOLOGICAL STACKS

- HTML
- CSS
- JavaScript
- Bootstrap
- PHP
- MySQL

## CONTRIBUTORS

- Kumar K Sir
- [Bhavdeep Singh Nijhawan](https://www.linkedin.com/in/bhavdeep-singh-nijhawan-739634280)

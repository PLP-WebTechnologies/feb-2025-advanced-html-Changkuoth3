# Advanced HTML5 Elements and Forms

## Objectives
Implement HTML5 images, lists, tables, forms and input types.
Use form validation attributes.
Apply multimedia elements such as audio and video.

## Instructions

- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form

>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 
# Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.

Happy Coding! 💻✨


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Kutey Web Page</title>
    <style>
        /* General body styling */
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        /* Main header styling */
        h1 {
            background-color: #4CAF50;
            color: white;
            text-align: center;
            padding: 10px 0;
        }

        /* Section styling */
        section {
            margin: 20px;
        }

        /* Table styling */
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
            background-color: white;
        }

        table, th, td {
            border: 1px solid #ddd;
        }

        th, td {
            padding: 12px;
            text-align: left;
        }

        /* Image styling */
        img {
            width: 100%;
            max-width: 600px;
            height: auto;
            display: block;
            margin: 0 auto;
        }

        /* Form styling */
        form {
            max-width: 600px;
            margin: 20px auto;
            padding: 20px;
            border: 1px solid #ddd;
            background-color: #fff;
            border-radius: 5px;
        }

        form input, form select, form textarea, form radio, form checkbox {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ddd;
            border-radius: 5px;
        }

        form input[type="submit"] {
            background-color: #4CAF50;
            color: white;
            border: none;
            cursor: pointer;
        }

        form input[type="submit"]:hover {
            background-color: #45a049;
        }

        label {
            font-weight: bold;
        }

        /* Styling for checkbox and radio buttons */
        .form-checkbox, .form-radio {
            display: inline-block;
            margin-right: 10px;
        }
    </style>
</head>
<body>

    <h1>Welcome to the Kutey Web Page</h1>

    <!-- Ordered List with Roman Numerals -->
    <section>
        <h2>Things to Do:</h2>
        <ol type="I">
            <li>Complete the Project</li>
            <li>Write and Test the Code</li>
            <li>Deploy the Website</li>
            <li>Promote the Application</li>
        </ol>
    </section>

    <!-- External Image -->
    <section>
        <h2>Beautiful Image from Pexels</h2>
        <img src="https://images.pexels.com/photos/3442314/pexels-photo-3442314.jpeg" alt="Beautiful Landscape from Pexels">
    </section>

    <!-- Table of Contacts -->
    <section>
        <h2>Contacts</h2>
        <table>
            <thead>
                <tr>
                    <th>Name</th>
                    <th>Address</th>
                    <th>Mobile</th>
                    <th>Email</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Boyaka Tiptip</td>
                    <td>123 Main St, Springfield</td>
                    <td>(555) 123-4567</td>
                    <td>boyaka.tiptip@email.com</td>
                </tr>
                <tr>
                    <td>Janes Dengh</td>
                    <td>456 Elm St, Shelbyville</td>
                    <td>(555) 987-6543</td>
                    <td>janes.deng@email.com</td>
                </tr>
                <tr>
                    <td>duol Joak</td>
                    <td>789 Oak St, Riverdale</td>
                    <td>(555) 555-5555</td>
                    <td>duol.joak@email.com</td>
                </tr>
                <tr>
                    <td>Hillary Tiptip</td>
                    <td>101 Pine St, Centerville</td>
                    <td>(555) 333-6666</td>
                    <td>hillary.tiptip@email.com</td>
                </tr>
                <tr>
                    <td>Them Gatjang</td>
                    <td>202 Maple St, Lakeside</td>
                    <td>(555) 444-7777</td>
                    <td>them.gatjang@email.com</td>
                </tr>
            </tbody>
        </table>
    </section>

    <!-- Registration Form -->
    <section>
        <h2>Registration Form</h2>
        <form action="#" method="post">
            <!-- Name Field -->
            <label for="name">Full Name:</label>
            <input type="text" id="name" name="name" placeholder="Enter your full name" required>

            <!-- Email Field -->
            <label for="email">Email Address:</label>
            <input type="email" id="email" name="email" placeholder="Enter your email" required>

            <!-- Password Field -->
            <label for="password">Password:</label>
            <input type="password" id="password" name="password" placeholder="Create a password" required>

            <!-- Date Field -->
            <label for="dob">Date of Birth:</label>
            <input type="date" id="dob" name="dob" required>

            <!-- Dropdown Field -->
            <label for="country">Select Your Country:</label>
            <select id="country" name="country" required>
                <option value="ssp">South sudan</option>
                <option value="kenya">Kenya</option>
                <option value="Egypt">Egypt</option>
                <option value="Ethiopia">Ethiopia</option>
            </select>

            <!-- Radio Button Field -->
            <label>Gender:</label>
            <div class="form-radio">
                <input type="radio" id="male" name="gender" value="male" required>
                <label for="male">Male</label>
            </div>
            <div class="form-radio">
                <input type="radio" id="female" name="gender" value="female">
                <label for="female">Female</label>
            </div>
            <div class="form-radio">
                <input type="radio" id="other" name="gender" value="other">
                <label for="other">Other</label>
            </div>

            <!-- Checkbox Field -->
            <label>Preferences:</label>
            <div class="form-checkbox">
                <input type="checkbox" id="newsletter" name="newsletter">
                <label for="newsletter">Sign up for the newsletter</label>
            </div>
            <div class="form-checkbox">
                <input type="checkbox" id="terms" name="terms" required>
                <label for="terms">I agree to the terms and conditions</label>
            </div>

            <!-- Submit Button -->
            <input type="submit" value="Register">
        </form>
    </section>

</body>
</html>


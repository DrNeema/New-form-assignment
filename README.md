# Form-assignment
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Registration Form</title>
    <!-- External Stylesheet Link -->
    <link rel="stylesheet" href="styles.css">
</head>

<body>
    <header>
        <h1>Registration Form</h1>
        <p>Please fill in the required fields.</p>
    </header>

    <!-- Form -->
    <form id="registrationForm" action="/submit" method="post">
        <!-- Personal Information Fieldset -->
        <fieldset>
            <legend>Personal Information</legend>

            <!-- First Name -->
            <label for="firstName">First Name:</label>
            <input type="text" id="firstName" name="firstName" required>
            <br><br>

            <!-- Last Name -->
            <label for="lastName">Last Name:</label>
            <input type="text" id="lastName" name="lastName" required>
            <br><br>

            <!-- Email -->
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            <br><br>

            <!-- Password -->
            <label for="password">Password:</label>
            <input type="password" id="password" name="password" 
                   pattern="^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)[A-Za-z\d]{8,}$" required>
            <small>Password must contain at least 8 characters, including one uppercase letter, one lowercase letter, and one number.</small>
            <br><br>
        </fieldset>

        <!-- Account Type Fieldset -->
        <fieldset>
            <legend>Account Type</legend>

            <!-- Radio Buttons for Account Type -->
            <label for="personalAccount">Personal Account:</label>
            <input type="radio" id="personalAccount" name="accountType" value="personal" required>
            <br><br>
            <label for="businessAccount">Business Account:</label>
            <input type="radio" id="businessAccount" name="accountType" value="business">
            <br><br>
        </fieldset>

        <!-- Profile Picture and Age Fieldset -->
        <fieldset>
            <legend>Profile Information</legend>

            <!-- File Input for Profile Picture -->
            <label for="profilePicture">Profile Picture:</label>
            <input type="file" id="profilePicture" name="profilePicture" accept="image/*">
            <br><br>

            <!-- Number Input for Age -->
            <label for="age">Age:</label>
            <input type="number" id="age" name="age" min="18" max="120" required>
            <br><br>
        </fieldset>

        <!-- Referrer and Bio Fieldset -->
        <fieldset>
            <legend>Referrer and Bio</legend>

            <!-- Referrer Dropdown -->
            <label for="referrer">How did you find us?</label>
            <select id="referrer" name="referrer">
                <option value="friend">Friend</option>
                <option value="search">Online Search</option>
                <option value="socialMedia">Social Media</option>
            </select>
            <br><br>

            <!-- Bio Textarea -->
            <label for="bio">Bio:</label>
            <input type="bio" name="bio" rows="4" cols="50" placeholder="Tell us about yourself"><input>
            <br><br>
        </fieldset>

        <!-- Additional Information Fieldset -->
        <fieldset>
            <legend>Additional Information</legend>

            <!-- Date of Birth Input -->
            <label for="dob">Date of Birth:</label>
            <input type="date" id="dob" name="dob" required>
            <br><br>

            <!-- Interests Checkboxes -->
            <label>Interests:</label>
            <input type="checkbox" id="coding" name="interests" value="coding">
            <label for="coding">Coding</label>
            <input type="checkbox" id="design" name="interests" value="design">
            <label for="design">Design</label>
            <input type="checkbox" id="reading" name="interests" value="reading">
            <label for="reading">Reading</label>
            <br><br>

            <!-- Country Dropdown with Groups -->
            <label for="country">Country:</label>
            <select id="country" name="country">
                <optgroup label="Africa">
                    <option value="Kenya">Kenya</option>
                    <option value="Uganda">Uganda</option>
                </optgroup>
                <optgroup label="Asia">
                    <option value="India">India</option>
                    <option value="China">China</option>
                </optgroup>
            </select>
            <br><br>
        </fieldset>

        <!-- Terms and Conditions Fieldset -->
        <fieldset>
            <legend>Terms and Conditions</legend>

            <!-- Checkbox for Terms -->
            <label for="terms">Accept Terms and Conditions:</label>
            <input type="checkbox" id="terms" name="terms" required>
            <label for="terms">I agree to the <a href="/terms" target="_blank">Terms and Conditions</a></label>
            <br><br>
        </fieldset>

        <!-- Submit Button -->
        <button type="submit">Submit</button>
    </form>
</body>

</html>
# New-form-assignment

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Registration Form</title>

    <style>
        body {
            font-family: Arial, sans-serif;
            background: #f4f4f4;
            padding: 20px;
        }
        form {
            background: white;
            padding: 20px;
            max-width: 400px;
            margin: auto;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        label {
            font-weight: bold;
            display: block;
            margin-top: 15px;
        }
        input, select, button {
            width: 100%;
            padding: 10px;
            margin-top: 5px;
        }
        button {
            background: #007bff;
            color: white;
            border: none;
            cursor: pointer;
            margin-top: 20px;
        }
        button:hover {
            background: #0056b3;
        }
    </style>
</head>
<body>

<h2>Student Registration Form</h2>

<form>
    <!-- Full Name -->
    <label for="name">Full Name:</label>
    <input type="text" id="name" name="name" 
           placeholder="Enter full name" 
           required minlength="3">

    <!-- Email -->
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" 
           placeholder="example@email.com" 
           required>

    <!-- Phone -->
    <label for="phone">Phone Number:</label>
    <input type="tel" id="phone" name="phone"
           placeholder="123-456-7890"
           pattern="[0-9]{3}-[0-9]{3}-[0-9]{4}"
           required>

    <!-- Date of Birth -->
    <label for="dob">Date of Birth:</label>
    <input type="date" id="dob" name="dob" required>

    <!-- Gender Dropdown -->
    <label for="gender">Gender:</label>
    <select id="gender" name="gender" required>
        <option value="">-- Select Gender --</option>
        <option value="Male">Male</option>
        <option value="Female">Female</option>
        <option value="Other">Other</option>
    </select>

    <!-- Course -->
    <label for="course">Course:</label>
    <select id="course" name="course" required>
        <option value="">-- Select Course --</option>
        <option value="Computer Science">Computer Science</option>
        <option value="Mathematics">Mathematics</option>
        <option value="Business Administration">Business Administration</option>
        <option value="Psychology">Psychology</option>
    </select>

    <!-- Password -->
    <label for="password">Create Password:</label>
    <input type="password" id="password" name="password"
           required minlength="6"
           pattern=".{6,}"
           placeholder="At least 6 characters">

    <!-- Submit -->
    <button type="submit">Register</button>
</form>

</body>
</html>
# student-registration

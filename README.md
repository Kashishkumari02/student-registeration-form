# student-registeration-form

A simple **Student Registration Form** desktop application built using **Java Swing**. This project demonstrates the use of Swing components, event handling, layouts, and form controls to create a basic graphical user interface (GUI).

## 📌 Project Overview

The Student Registration Form allows users to enter basic student information through a graphical interface.

The form contains:

* Student Name
* Roll Number
* Gender
* Branch
* Terms & Conditions checkbox
* Submit button
* Reset button

The project is designed to demonstrate the fundamentals of **Java GUI development using Swing**.

## 🛠️ Technologies Used

* **Java**
* **Java Swing**
* **AWT Event Handling**
* `JFrame`
* `JLabel`
* `JTextField`
* `JRadioButton`
* `ButtonGroup`
* `JCheckBox`
* `JButton`
* `ActionListener`

## 📂 Project Structure

```text
Student-Registration-Form/
│
├── StudentRegistration.java
└── README.md
```

## ✨ Features

### Student Name

A text field is provided to enter the student's name.

### Roll Number

A text field allows the user to enter the student's roll number.

### Gender Selection

The user can select either:

* Male
* Female

`ButtonGroup` is used so that only one gender option can be selected at a time.

### Branch

A text field is provided to enter the student's branch.

### Terms & Conditions

A checkbox allows the user to accept the Terms & Conditions.

### Reset Button

The **Reset** button clears:

* Student Name
* Roll Number
* Branch
* Gender selection
* Terms & Conditions selection

## 🖥️ User Interface

The application opens a window titled:

```text
Student Registration Form
```

The form is arranged using manually defined component positions with `setBounds()`.

## ▶️ How to Run

### 1. Install Java

Make sure Java JDK is installed on your computer.

Check the installation:

```bash
java -version
```

Check the Java compiler:

```bash
javac -version
```

### 2. Save the Java File

Save the program as:

```text
StudentRegistration.java
```

The filename must match the public class name:

```java
public class StudentRegistration
```

### 3. Compile the Program

Open a terminal in the project folder and run:

```bash
javac StudentRegistration.java
```

### 4. Run the Program

```bash
java StudentRegistration
```

The Student Registration Form window will open.

## 🔄 How the Reset Function Works

The Reset button uses `ActionListener` to detect when the button is clicked.

The input fields are cleared using:

```java
txtName.setText("");
txtRoll.setText("");
txtBranch.setText("");
```

The selected gender is cleared using:

```java
genderGroup.clearSelection();
```

The Terms & Conditions checkbox is cleared using:

```java
terms.setSelected(false);
```

## 📚 Concepts Demonstrated

This project helps demonstrate the following Java concepts:

* Object-Oriented Programming
* Classes and Objects
* Inheritance
* Interfaces
* Event Handling
* GUI Programming
* Java Swing Components
* `ActionListener`
* Radio Button Groups
* Text Fields
* Checkboxes
* Buttons
* JFrame configuration

## ⚠️ Current Limitation

The **Submit button** is currently created but does not perform an action because an `ActionListener` has not yet been attached to it.

The Reset button is connected using:

```java
reset.addActionListener(this);
```

A future improvement would be to add an action listener to the Submit button and display the entered student information.

## 🚀 Future Improvements

Possible improvements include:

* Add functionality to the Submit button.
* Validate empty input fields.
* Validate the roll number.
* Display submitted student information.
* Add more branches using a `JComboBox`.
* Improve the GUI design.
* Add database connectivity.
* Store registered student information.
* Add success and error messages.
* Improve the layout using `GridLayout` or `GridBagLayout`.

## 👨‍💻 Learning Outcome

This project provides practical experience in creating desktop applications using Java Swing and understanding how GUI components interact through event handling.

## 📄 License

This project is created for **educational and learning purposes**.

# rishitha
web cam security
# Web Cam Security Application

This is a Python-based desktop application designed for securing access to your webcam through OTP (One-Time Password) verification. The application allows you to send an OTP to a specified email address and, upon successful verification, provides options to enable or disable the webcam on a Windows system.

## Features

- **OTP Generation & Emailing**: 
  - Generates a 6-digit OTP.
  - Sends the OTP to a specified email address for verification.

- **OTP Verification**:
  - Verifies the user-input OTP against the generated OTP.

- **Webcam Control**:
  - Allows the user to check the current status of the webcam.
  - Provides options to enable or disable the webcam.

## Prerequisites

- **Python 3.x**: Make sure Python is installed on your system.
- **pip**: Ensure you have pip installed for managing Python packages.

## Installation

1. **Clone the repository**:

    ```bash
    git clone https://github.com/yourusername/webcam-security.git
    cd webcam-security
    ```

2. **Install required Python packages**:

    ```bash
    pip install customtkinter
    ```

## How to Run

1. **Run the application**:

    ```bash
    python webcam_security.py
    ```

2. **Usage**:
   - Enter your email address and click "Sign In" to receive an OTP.
   - Enter the received OTP in the designated field and click "Verify".
   - Upon successful verification, the application will show options to check, enable, or disable the webcam.

## Configuration

- **Email Sending**: 
  - The application uses Gmail's SMTP server. Replace the `sender_email` and `password` in the `send_email` function with your credentials. Ensure that "Less secure apps" access is enabled for your Gmail account or use an app password.

## Security Notes

- **Email Credentials**:
  - Be cautious with your email credentials. Do not hardcode them in the source code for production use. Consider using environment variables or secure vaults.

- **Admin Privileges**:
  - The commands to enable or disable the webcam may require administrator privileges. Run the script as an administrator to ensure proper functionality.

## Troubleshooting

- **Camera Not Responding**:
  - If the camera status is not updating, ensure that the necessary drivers are installed and that you have administrative privileges to execute PowerShell commands.

- **Email Not Received**:
  - Check your email credentials and ensure that the SMTP server settings are correct. Also, check your spam folder.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter) - For the modern-looking Tkinter widgets.
- [Python SMTP Library](https://docs.python.org/3/library/smtplib.html) - For sending emails.
- [PowerShell](https://docs.microsoft.com/en-us/powershell/) - For controlling the webcam.



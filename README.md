# Automatic Text Sender

This script automatically sends a "Good morning!" text message every day at 6:00 AM using the Textbelt API. The code is customizable, allowing you to modify the message content, recipient, and send time as needed.

## Prerequisites
- Python 3.x
- Libraries: `requests` and `schedule`. 

  **Installation**:
  - For macOS:
    ```
    pip3 install requests schedule 
    ```
  - For Windows:
    ```
    pip install requests schedule
    ```

## How to Use
1. Set up the `credentials.py` with the recipient's phone number.
2. Modify the message content, recipient, or send time in `automatic_text.py` as needed.
3. Run the `automatic_text.py` script.
4. The script will automatically send the text message at the specified time.

## Features
- Uses the Textbelt API for sending SMS.
- Uses the `schedule` library for easy scheduling of tasks.

## Limitations
- The Textbelt API allows only 1 free test text per day.

## Future Improvements
- Integrate with other SMS APIs for more flexibility.
- Add error handling for failed message sends.
- Allow users to specify multiple recipients.

## Customization
The script is designed for easy customization. You can modify:
- The message content by changing the `'message'` parameter in the `send_message` function.
- The recipient by updating the `phone_number` in `credentials.py`.
- The send time by adjusting the `schedule.every().day.at()` method.

By making these simple adjustments, you can tailor the script to fit various messaging needs beyond just sending a "Good morning!" text.

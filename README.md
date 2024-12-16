
# Email Filter with Telegram Integration

This Python script filters unique emails from a given input file based on a specified domain or ISP and sends the filtered results to a Telegram bot. It also allows sending multiple files from the current directory to Telegram.

## Features

- **Email Filtering**: Filters out unique emails containing a specified domain/ISP (e.g., `@gmail.com`).
- **Progress Bar**: Uses `tqdm` to display a progress bar while processing the email list.
- **ASCII Art Header**: Displays a fancy ASCII art header for a professional look.
- **Colorful Output**: Uses `termcolor` to add color to terminal output for better user experience.

## Prerequisites

- Python 3.x
- Libraries: `requests`, `tqdm`, `termcolor`

To install the required libraries, run:

```bash
pip3 install requests tqdm termcolor
```

## How to Use

1. Clone or download this repository.
2. Open a terminal and navigate to the project directory.
3. Run the script:

```bash
python3 emdatafiltred.py
```

4. When prompted:
    - Enter the name of your input file (e.g., `list.txt`).
    - Enter the domain/ISP to filter emails (e.g., `@gmail.com`).

The script will:
- Process the input file and filter emails containing the specified domain.
- Save the filtered emails to a new file.


## Example Output

After the script processes your file, you will see output similar to:

```
 __  __            ___       _ 
|  \/  |_ __      / _ \__  _/ |
| |\/| | '__|____| | | \ \/ / |
| |  | | | |_____| |_| |>  <| |
|_|  |_|_|        \___//_/\_\_|

Email Filter

🔄 Processing your input file...
✅ Filtered 15 unique email(s) containing '@gmail.com' and saved to list_filtered_gmail_com.txt
```

And in your Telegram chat, you will receive:
- The original file (`list.txt`).
- The filtered file (`list_filtered_gmail_com.txt`).
- A message with the script's path.

## Credits

Created by [@mr_0x1](https://github.com/Mr-0x1).

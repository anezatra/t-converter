# 𖤍 T-Converter Trojan Embedding Tool v1.0 Beta 𖤍
![banner image](https://github.com/anezatra/t-converter/blob/main/banner.jpg)
## What is a t-converter❔
This tool allows you to embed a trojan file into any desired file and convert it to PDF or JPG format. This way, you can disguise viruses such as EXE or APK files as PDFs or JPGs. Through extensive research, I discovered that an Android virus can also appear in JPG or PDF format. This tool is entirely my creation, and I do not provide information on how the APK is converted to this format. Additionally, for EXE files, the tool can use WinRAR, which is available on any computer, to perform the conversion without needing Wine or Windows API emulation. WinRAR compresses applications into SFX archives and converts them to the chosen extension (PDF or JPG). This feature makes it easier to deceive your targets. The program also works on various operating systems, including Windows, Kali Linux, and Termux. 

## T-Converter PRO v1.0 ☆

The APK conversion process is available in the T-Converter Pro version. The Pro version is available for a fee. You can contact me to purchase it.

- Click for the video of converting Apk to PDF with Pro. [open video](https://www.youtube.com/watch?v=39GzJzuA3FE&t=10s)

**Contact Information:**

- Email: [anezatra@gmail.com](mailto:anezatra@gmail.com)
- Telegram: [@anezatra](https://t.me/anezatra)

## How does t-converter work ⚙️
This process involves creating a Self-Extracting Archive (SFX) using the rar command. First, it checks if the rar command is available. If the command is found, preparations for creating the archive are made, and the configuration file (sfxconfig.txt) is read. After verifying the presence of this file, the necessary command to create the SFX archive is prepared and executed. Once the command runs, the archive is created successfully, and a success message is displayed upon completion. Finally, any required conversion operations are performed on the output file, and the final output is saved. This process ensures that all steps proceed smoothly and provides clear feedback to the user. </br>
```
+-----------------------------+        +-----------------------------+        +-----------------------------+
| Check if 'rar' command is   |        | Print message: "rar command |        | Read configuration file:    |
| available                   | -----> | interface available"        | -----> | sfxconfig.txt                |
+-----------------------------+        +-----------------------------+        +-----------------------------+
               |                                     |                                       |
               v                                     v                                       v
+-----------------------------+        +-----------------------------+        +-----------------------------+
| Check if SFX config file    |        | Print message: "Executing   |        | Prepare SFX archive command: |
| exists                      | -----> | SFX command"                 | -----> | 'rar a -sfx -z<sfx_path> -r  |
+-----------------------------+        +-----------------------------+        | <out_file> <exe_file> <pdf_file>'|
               |                                     |                                       |
               v                                     v                                       v
+-----------------------------+        +-----------------------------+        +-----------------------------+
| Execute SFX command         |        | Print message: "SFX archive |        | Perform file conversion and  |
|                             | -----> | created successfully!"       | -----> | save as final output         |
+-----------------------------+        +-----------------------------+        +-----------------------------+
               |                                     |                                       |
               v                                     v                                       v
+-----------------------------+        +-----------------------------+
| Print messages:             |        | End of process              |
| "Adding icon to the file"   |        |                             |
| "Created exe file converts  |        |                             |
| to pdf"                     |        |                             |
+-----------------------------+        +-----------------------------+
```

## How to download 💡
**Run setup.sh to install the program:** <br/><br/>
```bash
$ bash setup.sh
```
## Then run the program, the files you will use are in the same location as the program. 
```bash
$ python3 main.py
```

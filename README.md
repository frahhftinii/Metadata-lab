# Week 4: Metadata Analysis

## Tools Used
- exiftool
- hexeditor
- binwalk
- strings
- file

---

## Task

| Picture        | Tools        | Command / Link | Analysis |
|----------------|--------------|----------------|----------|
| Ocean.jpg      | exiftool     | https://exif.tools/ | EXIFTool is used to extract metadata such as date, camera model, and author. The image contains metadata that reveals information about how it was created. |
| Computer.jpg   | hexeditor    | https://hexed.it/ | The hex editor shows a PNG file signature (89 50 4E 47), indicating the file is actually a PNG even though it has a .jpg extension. |
| dog.jpg        | binwalk      | https://www.aperisolve.com/ | The result shows abnormal patterns and possible hidden layers, suggesting that the image may contain embedded or manipulated data (steganography). |
| Computer.jpg   | strings      | https://www.dcode.fr/strings-extractor | No significant readable strings were found, likely due to compression or encoding of the file. |
| solitaire.exe  | file         | https://www.checkfiletype.com/ | The file is detected as a PNG image even though it has a .exe extension. This demonstratspoofinwhere a file is disguised as an executable. |
| rubiks.jpg     | file         | https://www.checkfiletype.com/ | The file is identified as a PNG image although the extension is .jpg. This shows that file extensions can be manipulated and should not be trusted. |

---

## Proof of Concept (POC)

### Ocean.jpg (exiftool)
![Ocean](<img width="1373" height="954" alt="image" src="https://github.com/user-attachments/assets/122daf24-c7ad-444e-9782-248160100718" />

### Computer.jpg (hexeditor)
![Hex](<img width="1373" height="954" alt="image" src="https://github.com/user-attachments/assets/96356ba8-b88b-4d51-bc88-147503952eb1" />

### dog.jpg (binwalk)
![Binwalk](<img width="1373" height="954" alt="image" src="https://github.com/user-attachments/assets/2607a433-8d38-4f30-928e-08a627de5bb0" />

### Computer.jpg (strings)
![Strings](<img width="1373" height="954" alt="image" src="https://github.com/user-attachments/assets/32ca7d87-bbe7-46e5-b045-db17ada454d7" />

### solitaire.exe (file)
![Solitaire](<img width="1373" height="954" alt="image" src="https://github.com/user-attachments/assets/6d16e605-72a5-4051-b2f2-628d5168b6b9" />

### rubiks.jpg (file)
![Rubiks](<img width="1373" height="954" alt="image" src="https://github.com/user-attachments/assets/e4365fc1-0d28-46e3-a9b1-8440709e1b22" />

---

## Conclusion

This task demonstrates how different tools can be used to analyze metadata and detect hidden or manipulated data in files.

The findings show that:
- Metadata can reveal hidden information about an image (EXIFTool)
- File headers can expose the true file type (HexEditor)
- Hidden or suspicious data can be detected (Binwalk)
- Readable strings may or may not exist depending on encoding (Strings)
- File extensions can be easily manipulated and should not be trusted (File analysis)

👉 Therefore, multiple forensic tools must be used to verify file integrity and detect disguised or malicious files.

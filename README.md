# Week 4: Metadata Analysis

## Tools Used
- exiftool
- hexeditor
- binwalk
- strings

---

## Task

| Picture        | Tools        | Command / Link | Analysis |
|----------------|--------------|----------------|----------|
| Ocean.jpg      | exiftool     | https://exif.tools/ | EXIFTool is used to extract metadata such as date, camera model, and author. The image contains metadata that reveals information about how it was created. |
| Computer.jpg   | hexeditor    | https://hexed.it/ | The hex editor shows a PNG file signature (89 50 4E 47), indicating the file is actually a PNG even though it has a .jpg extension. |
| dog.jpg        | binwalk      | https://www.aperisolve.com/ | The result shows abnormal distortion, suggesting hidden or manipulated data within the image, indicating possible steganography. |
| Computer.jpg   | strings      | https://www.dcode.fr/strings-extractor | No significant readable strings were found, likely due to compression or encoding of the file. |


---

## Proof of Concept (POC)

### Ocean.jpg (exiftool)
![Ocean](<img width="1373" height="954" alt="image" src="https://github.com/user-attachments/assets/43396426-8263-4de0-9d95-b9020560fe82" />


### Computer.jpg (hexeditor)
![Hex](<img width="1373" height="954" alt="image" src="https://github.com/user-attachments/assets/7c3194eb-5d27-49a8-9380-30bb71d837f3" />


### dog.jpg (binwalk)
![Binwalk](<img width="1373" height="954" alt="image" src="https://github.com/user-attachments/assets/a88e8505-cd3d-4246-81b9-0bad0b77b2cc" />
![Binwalk](<img width="1373" height="954" alt="image" src="https://github.com/user-attachments/assets/d81487ab-bd21-4675-bf40-00b88f9e5820" />


### strings
![Strings](<img width="1373" height="954" alt="image" src="https://github.com/user-attachments/assets/ebaec54f-e7bc-4427-98c6-89e7c4d9af26" />


---

## Conclusion

This task demonstrates how different tools can be used to analyze metadata and detect hidden or manipulated data in files. It shows that file extensions can be misleading and emphasizes the importance of verifying file types using proper tools in digital forensics.

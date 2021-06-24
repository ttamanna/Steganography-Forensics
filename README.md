# Steganography Forensics

## Steganography
Steganography is the process of hiding an information in a file. It is one of the most important discovery which provides secrecy while transferring data or to protect against threats. In the same way, it can also be a lethal threat which can leave law enforcement and experts scratching their head. In today’s modern world where everything is connected to internet, steganography technique has also evolved and now it has not just become a medium to deliver secret messages but also a medium to inflict harm on others. Some of the major adversarial field impacted by it are pornography, terrorism, data theft and harm.


## Steganalysis
Steganalysis refers to the process of detection of the hidden information using steganography tools or techniques in media files. The main goal of a forensic examiner in this process is to detect and extract the hidden information reliably. This process requires knowledge of the original file, but that is not available in most cases. The features and characteristics of both the objects, stego- and coverobject are taken into consideration for steganalysis.

## Stego tools
The detection of steganography software on a suspect computer is important to the subsequent forensic analysis. As the research shows, many steganography detection programs work best when there are clues as to the type of steganography that was employed in the first place. Finding steganography software on a computer raises the possibility that the suspect computer contains steganography files containing secret messages.

* **Gargoyle (formerly StegoDetect):**
This tool can be used to detect the presence of steganography software. Gargoyle compares the hashes of the files under quest to a proprietary data set (or hash set) of all the files in the documented steganography software distributions. Cryptography, instant messaging, key logging, Trojan horses, password cracking, and other malicious malware can all be detected using Gargoyle data sets.

* **Stegdetect:**
Niels Provos' Stegdetect is a popular detection software. Stegdetect uses steganography schemes like F5, Invisible Secrets, JPHide, and JSteg to find hidden details in JPEG images (OutGuess 2003).

* **Stego Suite:**
Stego Suite is is comprised of Stego Watch, Stego Analyst and Stego Break. This tool can be used for investigation, detection, analysis, reporting as well as recovery of digital steganography. Stegowatch analyses collection of files to determine which are steganography media and the most likely algorithm for hiding them (which, in turn, provides clues as to the most likely software employed). The study employs a number of user-selectable statistical tests based on carrier file characteristics that may be affected by various steganography techniques. Stego break uses a dictionary attack to find the password of the hidden data against JSteg-Shell, JPHide, and OutGuess.

* **StegCracker:**
This tool can be used for dictionary attacks against steganographic files which are protected with passwords. After the attack, StegCracker automaticaaly writes the hidden data to an output file.

## Image Steganalysis
Steghide is used to embed a text to an image file. Here, ‘cat.jpg’ is the original file, ‘msg.txt’ is the secret information, and ‘stego.jpg’ is the steganographic image. The file is locked with the password ‘pass’.
![a](https://user-images.githubusercontent.com/79892851/123268747-abfce400-d541-11eb-87c8-af2026095c7d.PNG)

The Steganographic image appears larger in size and the hash values are different from the original image.
![b](https://user-images.githubusercontent.com/79892851/123269105-0138f580-d542-11eb-8e55-0a40db0245ad.PNG)
![c](https://user-images.githubusercontent.com/79892851/123269140-0b5af400-d542-11eb-830a-87fd8f92fb6b.PNG)

Stegcracker is used to attack the file against a wordlist. The conducted attack here is a dictionary attack against the wordlist ‘wordlist.txt’. The secret is extracted from the steganographic file successfully.Stegcracker automatically wrote the hidden information to a file ‘stego.jpg.out’. Both information matched and the attack was successful.
![d](https://user-images.githubusercontent.com/79892851/123269381-45c49100-d542-11eb-8a50-0a9620b362c2.PNG)


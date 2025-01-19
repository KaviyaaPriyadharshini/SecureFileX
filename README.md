# FileEncryption

A JavaFX Application that encrypts a file using AES encryption.

## Preview

![First screenshot of the application](https://raw.githubusercontent.com/luisbraganca/file-encryption/master/Screenshots/preview1.png)

![Second screenshot of the application](https://raw.githubusercontent.com/luisbraganca/file-encryption/master/Screenshots/preview2.png)

![Third screenshot of the application](https://raw.githubusercontent.com/luisbraganca/file-encryption/master/Screenshots/preview3.png)

## Technical details

This application allows you to encrypt a file using the [AES](https://en.wikipedia.org/wiki/Advanced_Encryption_Standard) encryption algorithm, asking you for a password to use it as its key. During the file transformation process, it's guaranteed that no data is lost: It's never the original file that is encrypted but a copy of it. And during the name changes, if there's already a file with that same name, a new one is used. For example:
* We have the file: Example.pdf
* If we encrypt it, it becomes. Example.pdf.enc
* Now if we decrypt it back, it won't replace the original Example.pdf, it will create a new one named "(1) Example.pdf", incrementing the number inside the parentheses untill it finds an unused file name.

### Functionalities

* File encryption (or safely cancel it without crashing the application)
* File decryption (or safely cancel it without crashing the application)
* Select the file using a file chooser
* Friendly graphical user interface showing the progress of the task
* Embedded web browser on the "about" pane that opens this GitHub page

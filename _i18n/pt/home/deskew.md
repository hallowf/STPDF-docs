Altough ScanToPDF has the ability to deskew images it can't do it withouth [Tesseract](https://github.com/tesseract-ocr/tesseract),
and tesseract is not shipped with the app, if you are on linux you can just install it with your package manager
on windows you can find installers [here](https://github.com/UB-Mannheim/tesseract/wiki)

Tesseract will also need to be in the environment PATH variable, to check it is available just open up a command line and type tesseract,
if it displays info and it's arguments then it's working

**If you are having trouble doing this please visit the [help](help/) section**
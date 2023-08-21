# Lao OCR Scan (Lao KYC Scanner)

The First Lao OCR and Face Liveliness. Which you can scan Lao ID card(White ID card and Green ID Card), Passport.
The package can extract necessary data.
And you also take liveliness and match image from kyc document to compare that is the right person using the document or not.

- This is the first version which can work with Lao ID and passport only, If you want me to develop more for Lao family book please support me! and let me know.
- you can contact me at *phoutthakonebcl@gmail.com

## Preview
![](https://github.com/Tonhbcl28/laoocr/blob/main/assets/images/laoocr.gif?raw=true)

## Features
Package can extract the data from document as the following:
- Document Number.
- Date of birth.
- Issued Date.
- Expired Date, etc.
- Can match image from kyc document and liveliness cam to compare that is right person or not.

## Getting started
Install the package and call the widget directly you will receive the result.
### install with flutter
```
flutter pub add laoocr
flutter pub get
```
### Then You have to import the package to your project
```
import 'package:laoocr/laoocr.dart';
```

## General Setup
- Requirement SDK minimum version 2.18 up.
### Android
Android folder at app/build.gradle, you have to config as following:

```
 android {
   defaultConfig {
     minSdkVersion 21
   }
 }  
```

### IOS
You must add camera permission to the info.plist file.

## Usage
You can call the widget and get the response after the KYC Scan.
Please find the example Code:
```
LaoOCRScan(
      onCapture: (res) {
        print('OCR result = $res');
        print('OCR img = ${res['kycImg']}'); //Uint8List
      },
      showPopBack: true,
      doFaceReg: true,
      onFaceReg: (data) {
        //liveliness status is Passed means real people, Fail means fake person
        print('liveliness data = $data'); //image as base 64
      },
      showRetakeBtn: true,
      showSubmitBtn: true,
      showFaceSubmitBtn: true,
      txtSubmit: 'Submit',
      btnSubmit: () {
        print('submitt');
      },
      txtSubmitOnFace: 'Done',
      btnSubmitOnFace: () {
        print('face liveliness submit');
      },
    )
```

## Donation - Support Me
# Lao QR
![](https://github.com/Tonhbcl28/laoocr/blob/main/assets/images/supportme.jpg?raw=true)
# Binance - BTC
![](https://github.com/Tonhbcl28/laoocr/blob/main/assets/images/binance.jpg?raw=true)

# ---Or---
<a href="https://www.buymeacoffee.com/phoutthako7" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>

## Additional information
This Package can help Lao developer to work with KYC document and it's very easy to use with the high performance.
It can save the company cost too much.
- This is the first version which can work with Lao ID and passport only, If you want me to develop more for Lao family book please support me! and let me know.
- you can contact me at *phoutthakonebcl@gmail.com
  Thank you so much 😘 (❁´◡`❁).

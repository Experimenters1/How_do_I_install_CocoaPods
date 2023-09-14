# How_do_I_install_CocoaPods
## How_do_I_install_CocoaPods?
#
### Install Homebrew on Mac : 

1. Install Homebrew:      https://brew.sh

2. Create .zshrc directory on terminal:  touch ~/.zshrc

3. Run this lines on terminal :    export PATH=/opt/homebrew/bin:$PATH
         source ~/.zshrc

4. Check If Homebrew is available:  brew help

5. Install Cocoapods, run on terminal:   brew install cocoapods

6. Now, Cocoapods is available

Install pods in your project:

1. Open your project folder at terminal.

2. Run on terminal “pod init” to create podfile.

3. Open pod file and insert any pod, for example, “PryntTrimmerView” : pod "PryntTrimmerView".

4. Run on terminal “pod install” to install pods.

5. Now, you can import pods into your project.

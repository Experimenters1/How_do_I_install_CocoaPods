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

#
### Package.swift
Tệp **Package.swift** thường được sử dụng trong các dự án Swift Package Manager (SPM). SPM là một công cụ được tích hợp sẵn trong Xcode để quản lý và cài đặt các gói thư viện Swift.
<div class="code-snippet">
  <pre>
    <code>
      var count = 5
      count = 10 // Giá trị của biến count được thay đổi thành 10
    </code>
  </pre>
  <button class="copy-button" data-clipboard-target=".code-snippet"></button>
</div> <br>

Nếu dự án của bạn sử dụng SPM và có một tệp **Package.swift**, bạn sẽ tìm thấy nó ở thư mục gốc của dự án của bạn. Thường, nó sẽ nằm cùng cấp với tệp ***.xcodeproj** hoặc ***.xcworkspace.**

Để tạo một tệp **Package.swift** mới trong một dự án, bạn có thể sử dụng lệnh sau trong Terminal:
   

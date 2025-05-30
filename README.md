# Housing Management System - Static Website Hosting on AWS S3

This project is a simple static website built using HTML and CSS to showcase a Housing Management System. The main objective is to demonstrate how a static website can be hosted using **Amazon S3 (Simple Storage Service)**.

---

## 🌐 Project Purpose

To showcase how to host a static website on **AWS S3**, which is a scalable object storage service from Amazon Web Services. This project is **not meant to function as a dynamic or backend system**, but instead to show the deployment of a front-end-only website.

---
## Features

- Display various types of houses with images
- User testimonials section
- Contact information and form layout
- Responsive and clean design

---

## Installation

1. Clone the repository:  
   `git clone https://github.com/janapalabhuvaneswar1234/Housing-management-system.git`  
2. Open the `index.html` file in your web browser to view the project.

---

## Usage

- Browse housing properties on the homepage  
- Navigate testimonials and contact pages via the menu  
- Modify `style.css` to customize the look and feel

---

---

## 🚀 Hosting on AWS S3 - Steps

1. **Create an S3 Bucket**
   - Go to the [AWS S3 Console](https://s3.console.aws.amazon.com/s3/)
   - Click "Create bucket"
   - Give your bucket a unique name
   - Uncheck "Block all public access"
   - Create the bucket

2. **Enable Static Website Hosting**
   - Go to the **Properties** tab of your bucket
   - Scroll to **Static website hosting**
   - Enable it
   - Set the index document as `index.html`

3. **Upload Files**
   - Go to the **Objects** tab
   - Upload `index.html`, `style.css`, and the `img/` directory

4. **Add Public Read Permissions**
   - Go to the **Permissions > Bucket Policy**
   - Add the following policy:

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::your-bucket-name/*"
    }
  ]
}


## Technologies Used

- HTML  
- CSS  

---

## Screenshots

*(Add screenshots here to showcase your project visuals)*

---

## Author

Bhuvaneswar Janapala

---

## License
MIT License

Copyright (c) 2025 Bhuvaneswar Janapala

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.


<!DOCTYPE html>
<html lang="en">
<head>
  
     
       
</head>
<body>

<h1>QR Code Generator in Python</h1>

<p>
This is a simple Python program that generates a QR code from a user-provided URL
and saves it as an image file on your system.
</p>

<h2>Features</h2>
<ul>
    <li>Takes a URL as user input</li>
    <li>Generates a QR code for the given URL</li>
    <li>Saves the QR code as a PNG image</li>
    <li>Uses the <strong>qrcode</strong> Python library</li>
</ul>

<h2>Requirements</h2>
<p>Ensure Python (3.x recommended) is installed.</p>
<p>Install the required library using:</p>

<pre><code>pip install qrcode[pil]</code></pre>

<h2>How the Program Works</h2>
<ol>
    <li>The user enters a URL.</li>
    <li>A QR code is generated for the URL.</li>
    <li>The QR code is saved as an image on the Desktop.</li>
    <li>A confirmation message is displayed.</li>
</ol>

<h2>File Path Used</h2>
<p>The QR code image is saved at:</p>

<pre><code>C:\Users\LENOVO\Desktop\qrcode.png</code></pre>

<p>You can change the file path in the code if needed.</p>

<h2>Usage</h2>
<ol>
    <li>Run the Python script.</li>
    <li>Enter the URL when prompted.</li>
    <li>Check your Desktop for the QR code image.</li>
</ol>

<h2>Sample Code</h2>

<pre><code>import qrcode

url = input("Enter the URL:").strip()
file_path = "C:\\Users\\LENOVO\\Desktop\\qrcode.png"

qr = qrcode.QRCode()
qr.add_data(url)

img = qr.make_image()
img.save(file_path)
print("QR code was generated!")</code></pre>

<h2>Output</h2>
<p>A PNG image containing the QR code of the entered URL.</p>

<h2>License</h2>
<p>This project is free to use for educational and personal purposes.</p>

</body>
</html>


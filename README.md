# Medical_Data_Extraction_Project
I developed this project by using Python. In this project we analyze the patient related document and convert it from pdf to jpg format. And extract the meaningful information from that document.

### Project Analogy:
The medical information of the patient that we are using is called front end. The backend is python program.
API is requesting python program for extracting fields from the medical document and the python program returns your response of the fields.

![Program analogy](https://user-images.githubusercontent.com/116663553/204216566-781d61d5-0120-4ca9-9558-689cdbc0e074.png)

We build the software extract pro which handles two types of documents i.e. patient's prescription and patient's details. It extract the meaningful information i.e. patient address, medicines, direction, and refill.

### Steps that we are taken in this project:

Step 1: Convert PDF file into an image file by using a python module pdf2image.
![step-1](https://user-images.githubusercontent.com/116663553/204217981-62ad9cbd-1e4a-40ee-9030-f26dcd80ac32.png)

Step 2: Extract text from image file by using a python module pytesseract and a google OCR engine.
![step-2](https://user-images.githubusercontent.com/116663553/204218105-e9da7239-12b7-4cf9-afca-98eaca2d0b45.png)

By extracting text from an image, we see a little problem in here. In this text extraction, the black area does not extracting the text. So, after Step 1,
Convert the original image into pixelated image by using a framework openCV and a python module CV2.
![in between step 1 and step 2](https://user-images.githubusercontent.com/116663553/204218283-9e480f25-05b3-45d0-9c5b-aec638644d1a.png)

Then we again apply the step 2.

Step 3: After extracting the text from image. It converts the text into structured data where we can extract individual fields such as patient name, patient address, medicines, and so on by using Regex (Regular Expression).
![step-3](https://user-images.githubusercontent.com/116663553/204218608-106dcdd9-bc75-46ff-b70a-0f218eb63633.png)


### Flow Chart of Medical Extraction Project:
![full process](https://user-images.githubusercontent.com/116663553/204218806-31f2c10a-3b8a-489c-a986-fcb55469d42e.png)

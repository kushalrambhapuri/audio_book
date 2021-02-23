# audio_book
This is your Audio Book where you can read your PDFs easily.
I have done it by using Pycharm which is a python code editor.
For the code I have used a pip (python installation package) which are **pip install pyttsx3** and **pip install PyPDF2**
I have installed both the packages in python terminal.
I have took a Object Oriented programming PDF for the project to put the project in your PDF go to file location where you have saved the project and from there you can put the PDF in your project this is the download link- https://www.tutorialspoint.com/object_oriented_python/object_oriented_python_tutorial.pdf
At the first we are importing pyttsx3 and importing PyPDF2.
To open the PDF I have created a variable called book and the value is open('**Here your PDF name should come**','rb').
And then we have created another variable called pdfReader and the value is PyPDF2.PdfFileReader(book).
And to show the number of pages in the PDF we have created another variable called pages and the value is pdfReader.numPages.
And then we are printing the variable pages to show the number of pages of the PDF.
And then again we have created another variable called speaker and the value is pyttsx3.init() here init means initiate.
Then we have created a for loop where the Audio Book reads the given PDF the for loop is for num in range(7, pages):
Then inside the for loop I have written page = pdfReader.getPage(7) and text = page.extractText() and speaker.say(text) and then at the last we have written as speaker.runAndWait().
And Yes!! Your Audio Book is ready no need to read books.

# WebPDF.js

Foxit WebPDF.js provides a world-class JavaScript library for viewing PDF files in web browsers. It requires no plug-ins and client side rendering -- it is a 100% JavaScript/HTML/CSS solution. Simply put, it offers the same power and accuracy as a desktop PDF viewer such as Foxit Reader, but for web browsers. For free!

WebPDF.js is based on Foxit’s advanced PDF engine, which is used by hundreds of millions of people and trusted by a large number of well-known companies around the world. Unlike other libraries such as PDF.js, WebPDF.js provides high fidelity PDF rendering inherited from it is market proven technology and it is engineered to be immune to browser variations in html5 support.

For developers who have implemented pdf.js in their projects but find the lack of accuracy and support troublesome, we have good news WebPDF.js provides an interface that you can use to migrate and replace pdf.js with no changes to your front-end code. It's ready to swap in and do the job you need it to in no time.

Following are the supported features:

- PDF viewing
- Go to page
- Zoom 
- Rotate page
- Page thumbnail
- Bookmark
- Access file attachments
- Text search
- Print selected pages
- Open password protected PDF
- Full-screen view
 


## Getting Started

### Online demo

+ http://184.105.214.152:8081/web/viewer.html

###Run up the package
   Unzip the package and then copy "webapp" and "build" folders to a web container;
   In a web browser, open http://{ip}:{port}/webapp/viewer.html to try out the viewer.
   
###Font server selection for non-embedded font files
WebPDF.js need to connect a server to download the font file if a PDF contains no-embedded fonts. We provide 2 public font servers, one each in US and China.

There are two pdf.workder.js files, WebPDF.workder.cn.js is for Chinese server, WebPDF.workder.us.js is for US server.

WebPDF.worker.us.js is used by default. You can easily change it to the Chinese font server with the following.
Find webapp/webpdf.config.js，

>    var WebPDF = {
    'workerSrc' : '../build/WebPDF.worker.us.js'
   };

 Replace WebPDF.worker.us.js to WebPDF.worker.cn.js, and then open "viewer.html" again.

###Get a official license for free
There is a default trial key file under folder build/lib/, please contact us for a full free key with ot watermark.

###Resouces description
    webapp/images		             image resources
    webapp/locale		             localization resources
    webapp/compressed.tracemonkey-pldi-09.pdf   A sample file open by default
    webapp/jquery.mini.js            jquery plug-in
    webapp/pdf.viewer.js             JavaScirpt file for front-end
    webapp/viewer.html	             Viewer.html
    webapp/viewer.css	             The css file of PDF.js
    webapp/webpdf.mini.css	         The css file of WebPDF.js
    build/pdf.worker.js              worker file created in the front-end, used for load FXJS_rel.js, and handle data request
    build/WeBPDF.js                  The interface layer of WebPDF
    build/lib/FXJS_rel.js            The core engine of WebPDF.js
    build/lib/brotli.js              brotli decompress plug-in, used for compress font file
    build/lib/key.txt                The license key file



## Contact

We would love to hear your feedback on this new project. And of course, if you require more advanced functionality -- we've got that too. Just reach out to us and we'll be happy to help you.

Email: <webpdfdemo@foxitsoftware.com>

[www.foxitsoftware.com](www.foxitsoftware.com)

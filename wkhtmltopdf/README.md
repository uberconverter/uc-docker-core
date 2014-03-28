wkhtmltopdf
===========

    docker run -v /home/anj/Documents/tmp:/out wkhtmltopdf wkhtmltopdf.sh http://www.google.com /out/output.pdf

Also, idea to extend this to render via a Wayback proxy, using:

    --proxy http://wayback.proxy:18090
    --custom-header Accept-Datetime "xxx"

(above from http://wkhtmltopdf.org/usage/wkhtmltopdf.txt)

i.e. service that takes a URL and a Datetime and renders to PDF.

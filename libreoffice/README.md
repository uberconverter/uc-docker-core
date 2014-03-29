
LibreOffice
-----------

    libreoffice --headless --convert-to pdf test.doc
    libreoffice --headless --convert-to odt test.pdf

Not clear how to list all filters.

UnoConv
-------
http://dag.wiee.rs/home-made/unoconv/

    unoconv -f odt -t template.ott -o resume.odt resume.tmp.odt
    unoconv -f pdf -t template.ott -o resume.pdf resume.odt
    unoconv -f html -t template.ott -o resume.html resume.odt
    unoconv -f doc -t template.ott -o resume.doc resume.odt

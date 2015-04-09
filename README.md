imagegrep-bash
==============
unix 'grep' a word inside pdf or image based on OCR

<img alt="" src="http://www.gifbin.com/bin/092014/1410513359_cat_vs_lemon.gif" style="height:150px"/>

no repo is complete without a catgif!

# Install

    wget https://github.com/coderofsalvation/imagegrep-bash/blob/master/imagegrep 
    chmod 755 imagegrep
    ./imagegrep foo.pdf invoice eng 

# Requirements

  * tesseract-ocr
  * imagemagick 

these packages can be installed using apt-get or yum

# Why 

To automate, categorize files and their destination folder.
Personally I use this to scrape my mailbox and copy invoice-attachments to a preferred folder on my harddrive.

    ./imagegrep mailbox/latest/foo.pdf && echo "grab your wallet!" && mv foo.pdf ~/admin/invoices/.

OCR usually fails in many cases, but sometimes knowing one word (and its length) is enough.

Creating a presentation
=======================

* reST
* images
* PDF
* linux


Content
=======

AWS.rst::

    AWS Overview
    ============

    * Elastic Cloud (EC2)
    * S3
    * CloudFront
    * Virtual Private Cloud (VPC)
    * Simple Email Service  (SES)
    * ...


    EC2 Instance
    ============

    * hardware
    * performance

    ...

Images
======

::

    AWS Console UI
    ==============

    .. image:: instances.png
       :width: 70%

    ...


Style
=====

* background image 4:3
* PDF style sheet::

    {"pageSetup": {
        "width": "16cm",
        "height": "12cm",
        "margin-top": "0cm",
        "margin-bottom": "0cm",
        "margin-left": "0cm",
        "margin-right": "0cm",
        "margin-gutter": "0cm",
        "spacing-header": "5mm",
        "spacing-footer": "5mm",
        "firstTemplate": "cutePage"
    },
    "pageTemplates" : {
        "cutePage": {
            "frames": [["10%", "10%", "80%", "80%"]],
            "showHeader": false,
            "showFooter": false,
            "background" : "background.png"
        }
    }
    }


PDF
===

* rst2pdf::

    apt-get install rst2pdf

* AWS.pdf::

    rst2pdf AWS.rst -b1 -s slides.style


Futher reading
==============

* http://code.google.com/p/rst2pdf/

* http://docutils.sourceforge.net/rst.html


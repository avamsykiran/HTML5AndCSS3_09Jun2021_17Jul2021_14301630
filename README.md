(https://github.com/avamsykiran/HTML5AndCSS3_09Jun2021_17Jul2021_14301630.git)

Lab Setup
----------------------------------------------------------

    Any Text Editor (notpead,notepad++,VSCode,.......)
    Browser         Chrome

HTML 5
-----------------------------------------------------------

    Hyper Text MarkUp Language

    it is a scripting - markup language.

    to be interpreted by softwares called browser that 
            parse these docuemtns and 
            render them.

    SGML            (specification for any markup languages)
        Standard General Mark Up Language

        1. we use tags to construct elements.
            
            <emp>
                <empid>101</empid>
                <ename>Vamsy</ename>
                <sal>1234</sal>
            </emp>

            <div>
                <p>This is a para<p>
            </div>

            elements:   emp ename   empid   sal div p
            opening tags:
                        <emp> <empid>   <ename> <sal>   <div>   <p>  
            closing tags:
                        </emp>  .....

        2. we use attributes to attach info to tag.

             <emp empid="101">
                <ename>Vamsy</ename>
                <sal>1234</sal>
            </emp>

            <div style="text-align:center">
                <p>a pra</p>
            </div>

            style and empid are attribute....!

        3.  each opening tag must have a closing tag
        4.  each attributes valeu must be placed in dbl quotes.
        5.  one SGML document can have one and only one root element.


    HTML and XML are the two languages that honor the SGML specifications.

        HTML
                is to create formatted documents that can
                be easily transported across a network of 
                machine having different os.


                passed over http protocol

                Hyper Text      ===     Hyper Media

                    text
                    formatted text
                    graphics
                    links

    HTML Docuemnt
    ----------------------------

        1. .htm     .html
        2. Root element of an html doc is <html></html>
        3. The html documents are case insensitive.


    Block vs Inline Element
    ------------------------------------

         ma block element acts as contaienr of inline elements.

         a block will always appear in a exlusive line
         and no two block elements appear side by side

         inline elements will alwasy appear one besides the other.

    Html Entities
    -------------------

        are used to render special chars:

        &rarr;
        &larr;
        &gt;
        &lt;
        &nbsp;

        ...etc

    Lists
   -------------------
        ol      ordered list            numbered

                type        1,a,i,I

        ul      unordered list          bullets

                type        circle,dot,square

            li  list item
                

        Nested List  = a list cna contain another list as a list item.

    Tables
    --------------------

        table
                sub-eleemnts
                    caption
                    thead
                    tbody
                    tfoot
                    tr

                attributes
                    border
                    width
                    height
                    cellspacing
                    cellpadding

        tr
                sub-elements
                    th
                    td

                            rowspan
                            colspan

    iframe
    ----------------------------------------
        an iframe is used to embed on web page into
        another web page.

        <iframe src="url" width="" height="" >
        </iframe>

    Links
    -----------------------------------------
        anchro element      a

            <a href="url" target="">Link Text</a>

            target      _self
                        _frameName
                        _blank

    div and span
    -------------------------------------------

        div is a block element used to 
            group a set of elements so that they
            can be treated as a unit while giving styles.

        span is a inline element used to 
            group a set of elements so that they
            can be treated as a unit while giving styles.

    Media Elements
    ---------------------------------------------

        img
                src             path of the image file
                width
                height
                alt             an alternate message incase th iamge loading fails.

        
        video
                controls        mentioning this attribs makes the playback control appera.

                source
                    src         path of the video file

        audio
                controls        mentioning this attribs makes the playback control appera.

                source
                    src         path of the audio file

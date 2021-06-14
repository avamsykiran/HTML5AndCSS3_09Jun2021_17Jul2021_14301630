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

        canvas  is used to draw a graphic dynamically using the Graphics api
                with any client script like vbscript/javascript

        svg     is used to render logo or animated graphics of svg.

    HTML 5 symatic eleemnts
    ------------------------------

        SEO -   Search Engine Optimization.

                web-crawling that traverses through all availble web sites,
                the words and sentence are subjected to page ranking 
                algorithmes.


        h1 to h6

        strong,em, mark,del,ins,addr,tel               <===> span

        header,article,aside,main,section,nav,footer    <===> div

    HTML Form Elements
    -------------------------------

        id      is an attribute to each and every html element
                to enables us to access that eleemnt in the client sciprt.
                it is not possible that two or more elements to have the same id.


        name    is an attribute to all form elements used access the submited
                data on the server side.

        form
                action      the url to whom the data has to be submited
                method      GET | POST 
                novalidate


        label       holds the field name        
                    for     refer to that form element it is attached to.

        button      type    button | reset | submit (default)
                    name
                    value
                    formaction   the url to whom the data has to be submited
                    formmethod   GET | POST 

        select      multiple
                    name
                    option
                        value
        
        textarea    rows
                    cols

        input       type    text/password/file/checkbox/radio/hidden
                            date/time/datetime-local/number/decimal/range
                            email

                    value                   hold the default value
                    placeholder             alternate for label, use give hints..etc


        html 5 form element validation attriubtes
        -----------------------------------------------------
            required
            min
            max
            minlength
            maxlength
            pattern

    HTML 5 API
    --------------------------------
        Web Storage     
            used for storing data on the client machine like cookies

        Drag and Drop
        
        Graphics                geerate dynamic graphics on canvas

        Geolocation             aquire the client gps location

        Web worker              enable executing heavy laoded jobs in background

    CSS
    ---------------------------------
        cascading Style Sheets

            used to style web pages.

            1. CSS isolates teh page content and the page style
            2. CSS bring uniform css properties to style each and every html element.


            Css is applied as
                1. inline-styles
                2. embeded styles
                3. external styles

            Inline Styles
            -------------------

                style attribute on any eleemnt to be styled

                <tagName style="css-property:value;css-property:value">
                </tagName>
                
                the style is applied only to that tag
                on which its is defined.

            Embeded Styles
            ----------------------

                style element in head element is used to apply
                embeded styles

                    <head>
                     ...
                     <style>
                        selector {
                            css-property:value
                        }
                     </style>
                    </head>

                each and every page must be applied with the
                individual style.

            External Styles
            ----------------------

                mystyle.css
                --------------
                        selector {
                            css-property:value
                        }
                

                <head>
                    <link rel="stylesheet" href="mystyle.css"/>
                </head>

        Style conflicts?
        ---------------------

            in the order of incusion, the styles that
            are close and newer will override the farther
            or the older styles.

        CSS Selectors
        ----------------------

            selector is a small string or expression that
            if matched by any element in a page, will be applied with the
            style enclosed in the selector.

            Tag Name Selectors
            -------------------
                each tag name itself acts like a selector

                tagName{
                    css-property:value
                }

                all those element whose tagNaem matches with the tagName
                in the style sheet is applied with the respective styling...!

            Attribute Name Selectors
            -----------------------------
                each attribute itelf acts like a selector

                [attributeName]{
                    css-property:value;
                }

              all those element that have the attribute mentioned as is
                in the style sheet, is applied with the respective styling...!

            Class Selectors
            ----------------------------

                is any user defined name of category.

                .className{
                    css-property:value;
                }

                any element which is having class="className" ,
                will be applied witht he rewpective style.

            Id Selectors
            ----------------------------

                as we know id is used to identify an element uniquly,
                no two eleemnts can have the saem id.

                if we wish to target a specific element only,
                then we style it using its id;

                #id{
                    css-property:value
                }

            Psudo Selectors
            ----------------------------

                are a few pre-defiend selectors
                that each work differently.

                each psudeo selector starts with a ':'

        CSS Operators and list of Psuedo Selectors
        --------------------------------------------

        CSS Properties
        ----------------------

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

        CSS Operators 
        --------------------------------------------

        s1		applies to elements that have s1 as tag name
        .s1		applies to elements that have s1 as class
        #s1		applies to elements that have s1 as id

        s1,s2	applies to elements that match both selectors
        s1 s2	applies to all elements that match s2 and are inside s1
        s1>s2	applies to all elements that match s2 whose parent is s1
        s1+s2	applies to all elements that match s2 and are immediately after s1
        s1~s2	applies to every element that match s2 and is preceded by s1

                        applies to all elements that have
                        ------------------------------------
        [s1]			 s1 as attribute
        [s1='v1']		 s1 attrib with v1 value
        [s1~='v1']		 s1 attrib value containes word v1
        [s1*='v1']		 s1 attrib value containes word v1
        [s1!='v1']		 s1 attrib value not equal to v1
        [s1^='v1']		 s1 attrib value starts with the word v1
        [s1$='v1']		 s1 attrib value ends with the word v1

        Psuedo selectors
        ----------------------------------------------------------------------------
        input:enabled	Selects every enabled <input> element
        p:first-child	Selects every <p> element that is the first child 
                        of its parent
        p::first-letter	Selects the first letter of every <p> element
        p::first-line	Selects the first line of every <p> element
        p:first-of-type	Selects every <p> element that is the first <p> 
                        element of its parent
        input:focus		Selects the input element which has focus
        a:hover			Selects links on mouse over
        input:in-range	Selects input elements with a value within a specified range

        input:indeterminate		
                        Selects input elements that are in an indeterminate state

        input:invalid	Selects all input elements with an invalid value
        input:optional	Selects input elements with no "required" attribute

        p:last-child	Selects every <p> element that is the last child of its parent
        p:last-of-type	Selects every <p> element that is the last <p> element of its parent

        a:link			Selects all unvisited links
        :not(p)			Selects every element that is not a <p> element
        p:nth-child(2)	Selects every <p> element that is the second child of its parent
        p:nth-last-child(2)	
                        Selects every <p> element that is the second child of its parent, 
                        counting from the last child

        p:nth-last-of-type(2)	
                        Selects every <p> element that is the second <p> element of its parent, 
                        counting from the last child
        p:nth-of-type(2)	
                        Selects every <p> element that is the second <p> element of its parent

        CSS - unit of measure
        -----------------------------------

        absolute		(irrespective of screen size)
            in
            mm              
            cm
            pt		1 in = 72 pt
            pc		1 in = 6  pc   1 pc = 12 pt
        
        relative 	(to screen size)
        
            px
            
            %
            
            em			relative the font-size
                        1 em = complete font-size
                                            
                        font-size: 12pt;
                        width: 8em;	8*12pt = 96pt;
                        
            vh			1% of viewport height
            vw			1% of viewport width
            vmin		min of vh or vw
                                                
        CSS font related properties
        -----------------------------------
            font-family
            font-size
            font-variant		normal or small-caps
            font-weight			bold or bolder or boldest 
                                or any number like 300,400,500..etc
            font-style			italic or oblique
             
        CSS Text related Proeprties
        -----------------------------------
            color
            direction
            letter-spacing
            word-spacing
            text-align
            text-indent
            text-decoration		none | underline | line-through | overline
            
======================================================================            
        Web Page (html document)
            1. heading bearing your name in bold capitals.
            2. following the heading a blue backgrounded para stating
                your skills (key-words)
            3. a section displaying your technical skills
            4. a section displaying your experience
            5. a section displaying your qualifcations
            6. a form to contact you.
======================================================================
        
        table related css prperties
        ------------------------------------
            border-collapse			collapse or seperate
            border-spacing
            caption-stde			top left right bottom
            
        CSS list related properties
        ----------------------------------

            list-style-type			disc	circle	square	none	for ul
                                    decimal							for ol
                                    decimal-leading-zero	
                                    lower-alpha
                                    upper-alpha
                                    lower-roman
                                    upper-roman
            list-style-position		outside or inside
            list-style-image:		url('imgs/note.png')
            marker-offset
            
        display css proeprty
        ------------------------------

            display:		none		block	inline	inline-block table-cell
            
        controlling scroll bars
        ------------------------------------
            
            overflow
                        visible
                        scroll
                        auto
                        hidden
        
        background proeprties
        -------------------------------------
            background-color
            opacity

            background-image
            background-repeat
            background-poisition

        Position property
        --------------------------------------

            relative
            absolute

        Responsive Design
        --------------------------------------

            @media          is a css decorator 
                            used to cosntruct media queries?

        CSS Animations
        --------------------------------------

            the css animations are executed
            as constant change in the value of 
            a proeprty or properties over time.
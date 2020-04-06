# frontend css code for the tooglenav without javascript
/*
html5doctor.com Reset Stylesheet
v1.6.1
Last Updated: 2010-09-17
Author: Richard Clark - http://richclarkdesign.com
Twitter: @rich_clark
*/

html, body, div, span, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
abbr, address, cite, code,
del, dfn, em, img, ins, kbd, q, samp,
small, strong, sub, sup, var,
b, i,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, figcaption, figure,
footer, header, hgroup, menu, nav, section, summary,
time, mark, audio, video {
margin:0;
padding:0;
border:0;
outline:0;
font-size:100%;
vertical-align:baseline;
background:transparent;
}

body {
line-height:1;
}

article,aside,details,figcaption,figure,
footer,header,hgroup,menu,nav,section {
display:block;
}

nav ul {
list-style:none;
}

blockquote, q {
quotes:none;
}

blockquote:before, blockquote:after,
q:before, q:after {
content:'';
content:none;
}

a {
margin:0;
padding:0;
font-size:100%;
vertical-align:baseline;
background:transparent;
}

/* change colours to suit your needs */
ins {
background-color:#ff9;
color:#000;
text-decoration:none;
}

/* change colours to suit your needs */
mark {
background-color:#ff9;
color:#000;
font-style:italic;
font-weight:bold;
}

del {
text-decoration: line-through;
}

abbr[title], dfn[title] {
border-bottom:1px dotted;
cursor:help;
}

table {
border-collapse:collapse;
border-spacing:0;
}

/* change border colour to suit your needs */
hr {
display:block;
height:1px;
border:0;
border-top:1px solid #cccccc;
margin:1em 0;
padding:0;
}

input, select {
vertical-align:middle;
}
/* my code */

@import url("https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css");

*{
    list-style: none;
    text-decoration: none;
    margin: 0;
    padding: 0;
}
.sidebar{
    position: fixed;
    left:-250px;
    width:250px;
    height:100%;
    background-color: rgb(21, 21, 43);
    transition: all .5s ease;
}
.sidebar header{
    font-size: 22px;
    text-align: center;
    line-height: 70px;
    background-color: rgb(94, 94, 160);
    user-select: none;
    color:rgb(2, 1, 10);
    font-weight: 700;
}
.sidebar ul a{
    display: block;
    height: 100%;
    width: 100%;
    line-height: 65px;
    font-size: 20px;
    color: white;
    padding-left: 40px;
    box-sizing: border-box;
    border-top: 1px solid rgb(14, 3, 31);
    transition: all .5s ease  ;
    border-bottom: 1px solid rgb(14, 3, 31);

}
ul li :hover  {
    padding-left: 70px;

}
.sidebar ul a i{
    margin-right: 16px;
}
#check{
    display: none;
}
label #btn,label #cancel{
    position: absolute;
    cursor: pointer;
    background-color: black;
    border-radius: 3px;
   

}
label #btn{
    left: 40px;
    top:25px;
    font-size: 30px;
    color:white;
    padding: 6px 12px;   
    transition: all .5s;
}
label #cancel{
    z-index:1111; 
    left:-195px;
    top:17px;
    font-size: 25px;
    color:white;
    padding: 4px 9px;
    transition: all .5s ease;
    
}
#check:checked ~.sidebar{
    left: 0;
}
#check:checked ~ #btn{
    left: 250px;
    opacity: 0;
    pointer-events: none;

}
#check:checked ~ label #cancel{
    left: 195px;
}
#check:checked ~ section{
    margin-left: 250px;
}
section{
    background: url("img/bck-com2.jpeg") no-repeat;
    background-position: center;
    background-size: cover;
    height: 100vh;
    transition: all .5s;
}

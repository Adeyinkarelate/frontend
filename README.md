# frontend css code for the tooglenav 

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

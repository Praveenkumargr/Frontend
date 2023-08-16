# Frontend
<!DOCTYPE html>
<html>
    <head>
        <title>flex</title>
        <style>
            *{
                box-sizing: border-box;
            }
            header{
                text-align: center;
                padding: 15px;
              
            }
            header img{
                animation-name: hea;
                animation-duration: 5s;
                animation-iteration-count: 1;

            }
            @keyframes hea{
                0%{margin-right: 100%;  }
                50%{margin-left: 100%; transform: rotatey(180deg); width: 350px;}                
                100%{position: relative;}

            }
            #navbar a{
                text-decoration: none;
                color: white;
                padding: 25px;
            }
            #navbar{
                background-color: black;
                padding: 25px;
            }
             a:hover{
                background-color: brown;
                
            }
            .con{
                display: flex;
                

            }
            .side{
                flex: 20%;
                border-right: 1px solid black;
                margin-top: 5px;
            }
            .main{
                flex: 80%;
            }
            .side h2{
                margin-left: 8px;
            }
            .side h3{
                margin-left: 16px;
            }
            .side input[type=checkbox], input[type=radio]{
                margin-left: 25px;
            }
            .main{
                margin-top: 15px;
                margin-left: 8px;
            }
            .con1{
                display: flex;
            }
            .dis{
                color: rgb(230, 105, 105);
                font-size: xx-large;
            }
            .rate{
                font-size: 50px;
                font-weight: 850;
            }
            .mrp{
                font-size: xx-large;
                color: rgb(160, 160, 160);
            }
            footer{
                text-align: center;
                padding: 30px;
                background-color: rgb(33, 33, 33);
                color: white;
            }
            #page{
                display: flex;
                margin-left: 300px;
                margin-bottom: 50px;
                margin-top: 50px;           

            } 
            #page div{
                padding: 10px;
                text-align: center;
                border: 1px solid black;
                border-collapse: collapse;
                cursor: pointer;

            }
            #page div:hover{
                color: red;
            }
            @media screen and (max-width:700px)  {
                #navbar, .con, .con1 {
                    flex-direction: column;
                    
                }
                .side{
                    border-right: 1px solid transparent;
                    border-bottom: 1px solid black;
                }
                #navbar a{
                    display: block;
                }
                header img{
                    width: 300px;
                }
                #page{
                    margin-left: 5px;
                }
                
                
            }
    
            
            
        </style>
    </head>
    <body>
        <header>
           
            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a9/Amazon_logo.svg/603px-Amazon_logo.svg.png" width="500px" height="150px" alt="">
        </header>
        <div id="navbar">
            <a href="#">Home</a>
            <a href="#">Products</a>
            <a href="#">Contact</a>
            <a href="#">Location</a>

        </div>
        <div class="con">
            <div class="side">
                <div class="short">
                 <h2>Short</h2>
                 <input type="radio" name="fil" id="fil">
                 <label for="fil">Low-Heigh</label><br>
                 <input type="radio" name="fil" id="pri">
                 <label for="pri">Heigh-Low</label><br>
                 <input type="radio" name="fil" id="rel">
                 <label for="rel">Relevance</label><br>
                 <input type="radio" name="fil" id="New">
                 <label for="New">New arival</label>
                </div>
                <div class="filter">
                    <h2>Filter</h2>
                    <h3>Brand</h3>
                    <input type="checkbox" name="so" id="so">
                    <label for="so">Sony</label><br>
                    <input type="checkbox" name="Sam" id="sam">
                    <label for="sam">Samsung</label><br>
                    <input type="checkbox" name="mi" id="mi">
                    <label for="mi">Mi</label><br>
                    <input type="checkbox" name="Vi" id="vi">
                    <label for="vi">Vivo</label><br>
                    <input type="checkbox" name="op" id="op">
                    <label for="op">Oppo</label>
                    <h3>Price</h3>
                    <input type="checkbox" name="1" id="1">
                    <label for="1">10,000.00-15,000.00</label><br>
                    <input type="checkbox" name="2" id="2">
                    <label for="2">15,000.00-30,000.00</label><br>
                    <input type="checkbox" name="3" id="3">
                    <label for="3">30,000.00-50,000.00</label><br>

                </div>
                

            </div>
            <div class="main">
                <div class="con1">
                 <div> <img src="https://m.media-amazon.com/images/I/81t-iyg0JfL._SL1500_.jpg" width="250px" height="250px" alt=""></div>
                  <div>
                    <p>Oppo F23 5G (Bold Gold, 8GB RAM, 256GB Storage) | 5000 mAh Battery with 67W SUPERVOOC Charger | 64MP Rear Triple AI Camera with Microlens | 6.72" FHD+ 120Hz Display | with Offers</p>
                     <span class="dis" >-14%</span>  <span class="rate"> <sup>₹</sup>24,999 </span><br>
                     <span class="mrp">M.R.P.: <sup>₹</sup><del> 28,999</del> </span> 
                    <p>
                        <img src="https://buybackboss.com/wp-content/uploads/2020/01/Amazon-prime-Logo-1024x640.png" width="90px" height="30px" alt="">
                        Get it by <span class=" date"> Tomorrow, 22 May </span> <br>
                        FREE Delivery by Amazon
                    </p>

                  </div>   

                </div> <hr>
                <div class="con1">
                    <div><img src="https://m.media-amazon.com/images/I/71AvQd3VzqL._SL1500_.jpg" width="250px" height="250px" alt=""></div>
                    <div>
                        <p>OnePlus Nord CE 2 Lite 5G (Blue Tide, 6GB RAM, 128GB Storage) </p>
                         <span class="dis" >-5%</span>  <span class="rate"> <sup>₹</sup>18,999 </span><br>
                         <span class="mrp">M.R.P.: <sup>₹</sup><del>19,999</del> </span> 
                        <p>
                            <img src="https://buybackboss.com/wp-content/uploads/2020/01/Amazon-prime-Logo-1024x640.png" width="90px" height="30px" alt="">
                            Get it by <span class=" date"> Tomorrow, 22 May </span> <br>
                            FREE Delivery by Amazon
                        </p>
    
                      </div> 

                </div>
                <div id="page">
                    <div style="border-radius:8px 0px 0px 8px ;">&#60; Previous</div>
                    <div>1</div>
                    <div>2</div>
                    <div>3</div>
                    <div>4</div>
                    <div>5</div>
                    <div>6</div>
                    <div>...</div>
                    <div style="border-radius: 0px 8px 8px 0px;">Next&#62;</div>

                </div>



            </div>

        </div>
        <footer>
            

          Conditions of Use & Sale  Privacy Notice Interest-Based Ads <br>
         © 1996-2023, Amazon.com, Inc. or its affiliates 
        </footer>
    </body>
</html>

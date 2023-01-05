
<!DOCTYPE html>
<html lang="en">
    <head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Justine Sestina</title>

    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.0/css/all.min.css">
</head>
<style>
    @import url('https://fonts.googleapis.com/css2?family=Lobster&display=swap');
:root{
    --white: #fff;
    --light: #eeeded;
    --orange: #FFA16C;
    --black: black;
}
body{
    background-color: var(--gray);
    font-family: system-ui;
    overflow: scroll;
    background:gray;
}
.container{
    width:1100px;
    border:5px solid var(--black);
    max-width: 1000%;
    margin:50px auto 0;
    display: grid;
    grid-template-columns: 300px auto 10px;
    padding:20px;
    border-radius: 100px;
    min-height: 80vh;
    top:0;
}
.container .menu{
    background-color: var(--white);
    border-top-left-radius: 30px;
    border-bottom-left-radius: 30px;
}
.container .cart{
    background-color: var(--white);
    border-top-right-radius: 30px;
    border-bottom-right-radius: 30px;
}
.container .center{
    background-color: var(--light);
    border-left: 1px solid var(--light);
    border-right: 1px solid var(--light);
}
/* menu */
.menu .logo{
    padding:20px;
    font-family: 'Lobster', cursive;
    font-size: xx-large;
    height:40px;
}
.menu .logo span{
    color: var(--orange);
}
.menu ul{
    padding:20px 0 20px 20px;
    list-style: none;
    border-bottom: 1px solid var(--light);
}
.menu ul li{
    padding:10px 0;
}
.menu ul li i{
    margin-right: 12px;
}
.menu ul li.active{
    color: var(--orange);
    border-right: 2px solid var(--orange);
}
.menu ul li:hover{
    color: var(--orange);
    border-right: 2px solid var(--orange);
}
/* end menu */
/* center */
    /* form */
.center .search{
    background-color: var(--white);
    padding:20px;
    height:40px;
}
.center .search .form{
    width:max-content;
    border:1px solid var(--light);
    border-radius: 20px;
    padding-left:15px;
    color:var(--light);
}
.center .search .form input{
    border:none;
    padding:0 10px;
    outline: none;
    width:100px;
}
.center .search .form button{
   border:none;
   background-color: var(--orange);
   color: var(--light);
   padding:10px 20px;
   border-radius: 20px;
}

    /* end form */

.center h2{
    padding:20px;
}
.center .list{
    padding:0 20px 20px;
    display: grid;
    grid-template-columns: auto auto;
    column-gap: 20px;
    row-gap: 20px;
}
.item{
    background-color: var(--white);
    display: grid;
    grid-template-columns: 20% auto;
    padding:10px;
    column-gap: 20px;
    border-radius: 20px;
}
.item .img img{
    height:70px;
}
.item .img{
    background-color: var(--light);
    border-radius: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
}
.item .content .title{
    font-weight: bold;
}
.item .content .des{
    font-size: small;
    opacity: 0.7;
    margin-top:5px;
}
.item .content .price{
    color:var(--orange);
    letter-spacing: 2px;
    font-weight: 500;
    font-size: small;
    margin-top:5px;
}
.item .count{
    width: 50px;
    border-radius: 10px;
    margin-right: 10px;
    padding:3px 5px;
    border:1px solid var(--light);
    outline: none;
     margin-top:5px;
}
.item .content .add{
    margin-top:5px;
    background-color: var(--orange);
    color:var(--white);
    padding:5px 10px;
    border:none;
    border-radius: 10px;
}
.item .content .remove{
    padding:5px;
    border:none;
    margin-top:5px;
    border-radius: 10px;
    display: none;
}

/* end center */
.cart .item{
    transition: 0.5s;
    border-bottom: 1px solid var(--light);
    display: grid;
}
.cart .name{
    padding:20px;
    height:40px;
    font-weight: bold;
    font-size: xx-large;
    border-bottom:1px solid var(--light);
}
.danger{
    box-shadow: 0 10px 10px var(--orange);
    transform: translate(0,-10px);
}
.cart  .add{
color:black;
}
.cart .remove{
    display: inline-block!important;
}
button{
cursor: pointer;;
}
.cart > .container{
    display: flex;
}
.qq{
    background-color: white;
}
</style>
<body>
    <div class="container">
        <div class="menu">
            <div class="logo">
                Justine's'<span>V sole</span>
            </div>
            <ul>
                <li class="active"><i class="fa-solid fa-house-user"></i> Home</li>
                <li><i class="fa-regular fa-user"></i> User</li>
                <li><i class="fa-solid fa-heart"></i> Favourite</li>
            </ul>
             <ul>
                <li><i class="fa-brands fa-tiktok"></i> Tiktok</li>
                <li><i class="fa-brands fa-facebook"></i> Facebook</li>
                <li><i class="fa-brands fa-instagram"></i> Instagram</li>
            </ul>
        </div>
        <div class="center">
            <div class="search">
                <div class="form">
                    <i class="fa-solid fa-magnifying-glass"></i>
                    <input type="text" placeholder="Search..?">
                    <button>Search</button>
                </div>
            </div>

            <h2>PRODUCTS</h2>
            <div class="list">
                <div class="item" data-key="1">
                    <div class="img">
                        <img src="https://images.vans.com/is/image/Vans/VN0005UF6QU-ALT1?wid=1600&hei=1600&fmt=jpeg&qlt=90&resMode=sharp2&op_usm=0.9,1.7,8,0&bgc=e5e5e9" alt="">
                    </div>
                    <div class="content">
                        <div class="title">vans 1</div>
                        <div class="des">
                            OLD SKOOL SHOE
                        </div>
                        <div class="price">₱6000.03</div>
                        <input type="number" class="count" min="1" value="1">
                        <button class="add">buy</button>
                        <button class="qq" onclick="window.location.href='1.html';">description</button>
                        <button class="remove" onclick="Remove(1)"><i class="fa-solid fa-trash-can"></i></button>
                    </div>
                </div>

                <div class="item" data-key="2">
                    <div class="img">
                        <img src="https://images.vans.com/is/image/Vans/VN0A7Q5D6QU-ALT1?wid=1600&hei=1600&fmt=jpeg&qlt=90&resMode=sharp2&op_usm=0.9,1.7,8,0&bgc=e5e5e9" alt="">
                    </div>
                    <div class="content">
                        <div class="title">vans 2</div>
                        <div class="des">
                            CHECKERBOARD CLASSIC SLIP-ON SHOE
                        </div>
                        <div class="price">₱10,000.03</div>
                        <input type="number" class="count" min="1" value="1">
                        <button class="add">buy</button>
                        <button class="add" onclick="window.location.href='2.html';">description</button>
                        <button class="remove" onclick="Remove(2)"><i class="fa-solid fa-trash-can"></i></button>
                    </div>
                </div>

                <div class="item" data-key="3">
                    <div class="img">
                        <img src="https://images.vans.com/is/image/Vans/VN0A5AO8BM8-ALT1?wid=1600&hei=1600&fmt=jpeg&qlt=90&resMode=sharp2&op_usm=0.9,1.7,8,0&bgc=e5e5e9" alt="">
                    </div>
                    <div class="content">
                        <div class="title">vans 3</div>
                        <div class="des">
                            COZY HUG CLASSIC SLIP-ON SHOE
                        </div>
                        <div class="price">₱5000.9</div>
                        <input type="number" class="count" min="1" value="1">
                        <button class="add">buy</button>
                        <button class="add" onclick="window.location.href='3.html';">description</button>
                        <button class="remove" onclick="Remove(3)"><i class="fa-solid fa-trash-can"></i></button>
                    </div>
                </div>
                
                <div class="item" data-key="4">
                    <div class="img">
                        <img src="https://images.vans.com/is/image/Vans/VN0A5KYCZF5-ALT1?wid=1600&hei=1600&fmt=jpeg&qlt=90&resMode=sharp2&op_usm=0.9,1.7,8,0&bgc=e5e5e9" alt="">
                    </div>
                    <div class="content">
                        <div class="title">vans 4</div>
                        <div class="des">
                            SK8-HI MTE-2 SHOE
                        </div>
                        <div class="price">₱6880.97</div>
                        <input type="number" class="count" min="1" value="1">
                        <button class="add">buy</button>
                        <button class="add" onclick="window.location.href='4.html';">description</button>
                        <button class="remove" onclick="Remove(4)"><i class="fa-solid fa-trash-can"></i></button>
                    </div>
                </div>

                <div class="item" data-key="5">
                    <div class="img">
                        <img src="https://images.vans.com/is/image/Vans/VN0A5KYCPBQ-ALT1?wid=1600&hei=1600&fmt=jpeg&qlt=90&resMode=sharp2&op_usm=0.9,1.7,8,0&bgc=e5e5e9" alt="">
                    </div>
                    <div class="content">
                        <div class="title">vans 5</div>
                        <div class="des">
                            SK8-HI MTE-2 SHOE
                        </div>
                        <div class="price">₱6000.03</div>
                        <input type="number" class="count" min="1" value="1">
                        <button class="add">buy</button>
                        <button class="add" onclick="window.location.href='5.html';">description</button>
                        <button class="remove" onclick="Remove(5)"><i class="fa-solid fa-trash-can"></i></button>
                    </div>
                </div>

 <div class="item" data-key="6">
                    <div class="img">
                        <img src="https://images.vans.com/is/image/Vans/VN0A3D29SAG-ALT1?wid=1600&hei=1600&fmt=jpeg&qlt=90&resMode=sharp2&op_usm=0.9,1.7,8,0&bgc=e5e5e9" alt="">
                    </div>
                    <div class="content">
                        <div class="title">vans 6</div>
                        <div class="des">
                            SUEDE CANVAS OLD SKOOL V SHOE
                        </div>
                        <div class="price">₱12000</div>
                        <input type="number" class="count" min="1" value="1">
                        <button class="add">buy</button>
                        <button class="add" onclick="window.location.href='6.html';">description</button>
                        <button class="remove" onclick="Remove(6)"><i class="fa-solid fa-trash-can"></i></button>
                    </div>
                </div>
 
                <div class="item" data-key="7">
                    <div class="img">
                        <img src="https://images.vans.com/is/image/Vans/VN0A7Q5DBLL-ALT1?wid=1600&hei=1600&fmt=jpeg&qlt=90&resMode=sharp2&op_usm=0.9,1.7,8,0&bgc=e5e5e9" alt="">
                    </div>
                    <div class="content">
                        <div class="title">vans 7</div>
                        <div class="des">
                            CHECKERBOARD CLASSIC SLIP-ON SHOE
                        </div>
                        <div class="price">₱8000.67</div>
                        <input type="number" class="count" min="1" value="1">
                        <button class="add">buy</button>
                        <button class="add" onclick="window.location.href='7.html';">description</button>
                        <button class="remove" onclick="Remove(7)"><i class="fa-solid fa-trash-can"></i></button>
                    </div>
                </div>
        
  <div class="item" data-key="8">
                <div class="img">
                    <img src="https://images.vans.com/is/image/Vans/VN0A4U16861-ALT1?wid=1600&hei=1600&fmt=jpeg&qlt=90&resMode=sharp2&op_usm=0.9,1.7,8,0&bgc=e5e5e9" alt="">
                </div>
                <div class="content">
                    <div class="title">vans 8</div>
                    <div class="des">
                        SUEDE/CANVAS SK8-HI TAPERED SHOE
                    </div>
                    <div class="price">₱5060.03</div>
                    <input type="number" class="count" min="1" value="1">
                    <button class="add">buy</button>
                    <button class="add" onclick="window.location.href='8.html';">description</button>
                    <button class="remove" onclick="Remove(8)"><i class="fa-solid fa-trash-can"></i></button>
                </div>
            </div>
     
            <div class="item" data-key="9">
                <div class="img">
                    <img src="https://images.vans.com/is/image/Vans/VN0A5KS9BLL-ALT1?wid=1600&hei=1600&fmt=jpeg&qlt=90&resMode=sharp2&op_usm=0.9,1.7,8,0&bgc=e5e5e9" alt="">
                </div>
                <div class="content">
                    <div class="title">vans 9</div>
                    <div class="des">
                        AUTHENTIC SHOE
                    </div>
                    <div class="price">₱4600.03</div>
                    <input type="number" class="count" min="1" value="1">
                    <button class="add">buy</button>
                    <button class="add" onclick="window.location.href='9.html';">description</button>
                    <button class="remove" onclick="Remove(9)"><i class="fa-solid fa-trash-can"></i></button>
                </div>
            </div>

            <div class="item" data-key="10">
                <div class="img">
                    <img src="https://images.vans.com/is/image/Vans/VN0A7TNLRV2-ALT1?wid=1600&hei=1600&fmt=jpeg&qlt=90&resMode=sharp2&op_usm=0.9,1.7,8,0&bgc=e5e5e9" alt="">
                </div>
                <div class="content">
                    <div class="title">vans 10</div>
                    <div class="des">
                        FRESHMAN LOWLAND CC SHOE
                    </div>
                    <div class="price">5800</div>
                    <input type="number" class="count" min="1" value="1">
                    <button class="add">buy</button>
                    <button class="add" onclick="window.location.href='10.html';">description</button>
                    <button class="remove" onclick="Remove(10)"><i class="fa-solid fa-trash-can"></i></button>
                </div>
            </div>

            <div class="item" data-key="11">
                <div class="img">
                    <img src="https://images.vans.com/is/image/Vans/VN0A7TNL1NU-ALT1?wid=1600&hei=1600&fmt=jpeg&qlt=90&resMode=sharp2&op_usm=0.9,1.7,8,0&bgc=e5e5e9" alt="">
                </div>
                <div class="content">
                    <div class="title">vans 11</div>
                    <div class="des">
                        POP LOWLAND CC SHOE  
                    </div>
                    <div class="price">₱10800.03</div>
                    <input type="number" class="count" min="1" value="1">
                    <button class="add">buy</button>
                    <button class="add" onclick="window.location.href='11.html';">description</button>
                    <button class="remove" onclick="Remove(11)"><i class="fa-solid fa-trash-can"></i></button>
                </div>
            </div>

            <div class="item" data-key="12">
                <div class="img">
                    <img src="https://images.vans.com/is/image/Vans/VN000EYEW00-ALT1?wid=1600&hei=1600&fmt=jpeg&qlt=90&resMode=sharp2&op_usm=0.9,1.7,8,0&bgc=e5e5e9" alt="">
                </div>
                <div class="content">
                    <div class="title">vans 12</div>
                    <div class="des">
                        SLIP-ON SHOE
                    </div>
                    <div class="price">₱4000.03</div>
                    <input type="number" class="count" min="1" value="1">
                    <button class="add">buy</button>
                    <button class="add" onclick="window.location.href='12.html';">description</button>
                    <button class="remove" onclick="Remove(12)"><i class="fa-solid fa-trash-can"></i></button>
                </div>
            </div>

            <div class="item" data-key="13">
                <div class="img">
                    <img src="https://images.vans.com/is/image/Vans/VN0A7Q5M6BT-ALT1?wid=1600&hei=1600&fmt=jpeg&qlt=90&resMode=sharp2&op_usm=0.9,1.7,8,0&bgc=e5e5e9" alt="">
                </div>
                <div class="content">
                    <div class="title">vans 13</div>
                    <div class="des">
                        OLD SKOOL STACKFORM SHOE
                    </div>
                    <div class="price">₱13000</div>
                    <input type="number" class="count" min="1" value="1">
                    <button class="add">buy</button>
                    <button class="add" onclick="window.location.href='13.html';">description</button>
                    <button class="remove" onclick="Remove(13)"><i class="fa-solid fa-trash-can"></i></button>
                </div>
            </div>

            <div class="item" data-key="14">
                <div class="img">
                    <img src="https://images.vans.com/is/image/Vans/VN000D5IB8C-ALT1?wid=1600&hei=1600&fmt=jpeg&qlt=90&resMode=sharp2&op_usm=0.9,1.7,8,0&bgc=e5e5e9" alt="">
                </div>
                <div class="content">
                    <div class="title">vans 14</div>
                    <div class="des">
                        SK8-HI SHOE
                    </div>
                    <div class="price">₱8200.93</div>
                    <input type="number" class="count" min="1" value="1">
                    <button class="add">buy</button>
                    <button class="add" onclick="window.location.href='14.html';">description</button>
                    <button class="remove" onclick="Remove(14)"><i class="fa-solid fa-trash-can"></i></button>
                </div>
            </div>

            <div class="item" data-key="15">
                <div class="img">
                    <img src="https://images.vans.com/is/image/Vans/VN0A7TNOBMV-ALT1?wid=1600&hei=1600&fmt=jpeg&qlt=90&resMode=sharp2&op_usm=0.9,1.7,8,0&bgc=e5e5e9" alt="">
                </div>
                <div class="content">
                    <div class="title">vans 15</div>
                    <div class="des">
                        SHOWCASE COMFYCUSH SK8-HI SHOE
                    </div>
                    <div class="price">₱10000</div>
                    <input type="number" class="count" min="1" value="1">
                    <button class="add">buy</button>
                    <button class="add" onclick="window.location.href='15.html';">description</button>
                    <button class="remove" onclick="Remove(15)"><i class="fa-solid fa-trash-can"></i></button>
                </div>
            </div>

            <div class="item" data-key="16">
                <div class="img">
                    <img src="https://images.vans.com/is/image/Vans/VN0A5JMKW00-ALT1?wid=1600&hei=1600&fmt=jpeg&qlt=90&resMode=sharp2&op_usm=0.9,1.7,8,0&bgc=e5e5e9" alt="">
                </div>
                <div class="content">
                    <div class="title">vans 16</div>
                    <div class="des">
                        SK8-HI TAPERED STACKFORM SHOE
                    </div>
                    <div class="price">₱6500.03</div>
                    <input type="number" class="count" min="1" value="1">
                    <button class="add">buy</button>
                    <button class="add" onclick="window.location.href='16.html';">description</button>
                    <button class="remove" onclick="Remove(16)"><i class="fa-solid fa-trash-can"></i></button>
                </div>
            </div>

            <div class="item" data-key="17">
                <div class="img">
                    <img src="https://images.vans.com/is/image/Vans/VN000EE3WHT-ALT1?wid=1600&hei=1600&fmt=jpeg&qlt=90&resMode=sharp2&op_usm=0.9,1.7,8,0&bgc=e5e5e9" alt="">
                </div>
                <div class="content">
                    <div class="title">vans 17</div>
                    <div class="des">
                        AUTHENTIC SHOE
                    </div>
                    <div class="price">₱4600.53</div>
                    <input type="number" class="count" min="1" value="1">
                    <button class="add">buy</button>
                    <button class="add" onclick="window.location.href='17.html';">description</button>
                    <button class="remove" onclick="Remove(17)"><i class="fa-solid fa-trash-can"></i></button>
                </div>
            </div>

            <div class="item" data-key="18">
                <div class="img">
                    <img src="https://images.vans.com/is/image/Vans/VN0A5FCBNAV-ALT1?wid=1600&hei=1600&fmt=jpeg&qlt=90&resMode=sharp2&op_usm=0.9,1.7,8,0&bgc=e5e5e9" alt="">
                </div>
                <div class="content">
                    <div class="title">vans 18</div>
                    <div class="des">
                        SKATE OLD SKOOL SHOE
                    </div>
                    <div class="price">₱5000.88</div>
                    <input type="number" class="count" min="1" value="1">
                    <button class="add">buy</button>
                    <button class="add" onclick="window.location.href='18.html';">description</button>
                    <button class="remove" onclick="Remove(18)"><i class="fa-solid fa-trash-can"></i></button>
                </div>
            </div>

            <div class="item" data-key="19">
                <div class="img">
                    <img src="https://images.vans.com/is/image/Vans/VN0A5FCC17P-ALT1?wid=1600&hei=1600&fmt=jpeg&qlt=90&resMode=sharp2&op_usm=0.9,1.7,8,0&bgc=e5e5e9" alt="">
                </div>
                <div class="content">
                    <div class="title">vans 19</div>
                    <div class="des">
                        SKATE SK8-HI SHOE 
                    </div>
                    <div class="price">₱9900</div>
                    <input type="number" class="count" min="1" value="1">
                    <button class="add">buy</button>
                    <button class="add" onclick="window.location.href='19.html';">description</button>
                    <button class="remove" onclick="Remove(19)"><i class="fa-solid fa-trash-can"></i></button>
                </div>
            </div>

            <div class="item" data-key="20">
                <div class="img">
                    <img src="https://images.vans.com/is/image/Vans/VN0A7TNOBMV-ALT1?wid=1600&hei=1600&fmt=jpeg&qlt=90&resMode=sharp2&op_usm=0.9,1.7,8,0&bgc=e5e5e9" alt="">
                </div>
                <div class="content">
                    <div class="title">vans 20</div>
                    <div class="des">
                        SHOWCASE COMFYCUSH SK8-HI SHOE
                    </div>
                    <div class="price">₱10000</div>
                    <input type="number" class="count" min="1" value="1">
                    <button class="add">buy</button>
                    <button class="add" onclick="window.location.href='20.html';">description</button>
                    <button class="remove" onclick="Remove(20)"><i class="fa-solid fa-trash-can"></i></button>
                </div>
            </div>




        </div>
        <div class="cart">
            <div class="name">LIST BUY</div>
            <div class="listCart">

            </div>
        </div>
    </div>
     <script>
        let list = document.querySelectorAll('.list .item');
list.forEach(item => {
    item.addEventListener('click', function(event){
        if(event.target.classList.contains('add')){
            var itemNew = item.cloneNode(true);
            let checkIsset  = false;

            let listCart = document.querySelectorAll('.cart .item');
            listCart.forEach(cart =>{
                if(cart.getAttribute('data-key') == itemNew.getAttribute('data-key')){
                    checkIsset = true;
                    cart.classList.add('danger');
                    setTimeout(function(){
                        cart.classList.remove('danger');
                    },1000)
                }
            })
            if(checkIsset == false){
                document.querySelector('.listCart').appendChild(itemNew);
            }

        }
    })
})
function Remove($key){
    let listCart = document.querySelectorAll('.cart .item');
    listCart.forEach(item => {
        if(item.getAttribute('data-key') == $key){
            item.remove();
            return;
        }
    })
} 
     </script>
</body>
</html>

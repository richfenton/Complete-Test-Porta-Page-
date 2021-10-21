# Complete-Test-Portal-Page-
This is the full script for the portal test page (RF Generic (Test)) with Settlement option

HTML

<!DOCTYPE html>
<html>
<body>
***// Below is the code //***
<div class="topnav">
  <a class="active" href="https://zincaccountmanager.com/">Log Out</a>
	<a href="https://zincaccountmanager.com/">Home Page</a>
  <a href="https://zincaccountmanager.com/contact-us/">Contact Us</a>
</div>

<!-- Start of LiveChat (www.livechatinc.com) code -->
<script>
    window.__lc = window.__lc || {};
    window.__lc.license = 11334778;
    ;(function(n,t,c){function i(n){return e._h?e._h.apply(null,n):e._q.push(n)}var e={_q:[],_h:null,_v:"2.0",on:function(){i(["on",c.call(arguments)])},once:function(){i(["once",c.call(arguments)])},off:function(){i(["off",c.call(arguments)])},get:function(){if(!e._h)throw new Error("[LiveChatWidget] You can't use getters before load.");return i(["get",c.call(arguments)])},call:function(){i(["call",c.call(arguments)])},init:function(){var n=t.createElement("script");n.async=!0,n.type="text/javascript",n.src="https://cdn.livechatinc.com/tracking.js",t.head.appendChild(n)}};!n.__lc.asyncInit&&e.init(),n.LiveChatWidget=n.LiveChatWidget||e}(window,document,[].slice))
</script>
<noscript><a href="https://www.livechatinc.com/chat-with/11334778/" rel="nofollow">Chat with us</a>, powered by <a href="https://www.livechatinc.com/?welcome" rel="noopener nofollow" target="_blank">LiveChat</a></noscript>
<!-- End of LiveChat code -->


<body>
    <div class="tcontainer">
        <div class="ticker-wrap">
            <div class="ticker-move">
                <div class="ticker-item">{{Forename}} you can settle your account with a one off payment of £{{settle}} - Payment can be made below.</div>
								<div class="ticker-item">{{Forename}} you can settle your account with a one off payment of £{{settle}} - Payment can be made below.</div>
            </div>
        </div>
    </div>


### Welcome {{Forename}}
### Our Client - {{ContractLetterName}}
### Balance - £{{Balance}} 
### Minimum Payment - £{{min_due}} 


<div class="button-container">
  <div class="tile">
			<a href="/customerportal/payusingsagepay?numberofpayments=12&paymentfrequency=4&paymentdate={{payment_date}}&overrideAmount={{Balance}}&forceRegular=true&minimumPayment={{min_due}}&forcecpa=true" ><i class="fas fa-credit-card" aria-hidden="true"></i><p>Set Up A Payment Plan - Your Minimum Payment Is £{{min_due}}</p></a></div></div>
			
<div class="button-container">
  <div class="tile">
			<a href="/customerportal/payusingsagepay?numberofpayments=12&paymentfrequency=4&paymentdate={{payment_date}}&overrideAmount={{min_due}}&minimumPayment={{min_due}}&forceSingle=true" ><i class="fas fa-credit-card" aria-hidden="true"></i><p>Make Single Payment - Your Minimum Payment is £{{min_due}}</p></a>
	</div>
</div>


</body>
</html>
  
  ******Style sheets start Below******
  
  body {background-image:url(https://zincaccountmanager.com/wp-content/uploads/2021/10/Watermark-Two.png); 
      background-size: cover; 
      background-size: cover;
      background-repeat:no-repeat;
      color: #0076C1;
}
      

.logo { border-color:#0076C1 }

.tile {
   display: inline-block;
   height: 130px;
   list-style-type: none;
   margin: 10px 40px 10px 20px;
   position: relative;
   text-align: center;
   width: 270px;
   border-radius: 25px; !important;
}

.button-container {
  display: inline-block !important;
}

.tile a {text-align: center;
  width: 300px; height: 90px !important;
}
 
.tile a {background-color: #7D317A;
  background-image: linear-gradient(#0076C1, #0076C1, #0076C1 );}

 .tcontainer {
        width: 100%;
        overflow: hidden;
    }

    
    .ticker-wrap {
        width: 100%;
        padding-left: 100%;
        background-color: none;
    }
    
    @keyframes ticker {
        100% {
            transform: translate3d(-100%, 0, 0);
        }
    }
    
    .ticker-move {
        display: inline-block;
        white-space: nowrap;
        padding-right: 100%;
        animation-timing-function: linear;
        animation: ticker 40s linear infinite;
    }
    
    .ticker-move:hover {
        animation-play-state: running;
    }
    
    .ticker-item {
        display: inline-block;
        padding: 0 40px;
        font-size: 25px;
        font-weight: bold;
        color: #0076C1 !important;
    }



.topnav {
  overflow: hidden;
  background-color: #0076C1;
}

.topnav a {
  float: left;
  color: #FFFFFF;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
}

.topnav a:hover {
  background-color: #ddd;
  color: black;
}

.topnav a.active {
  background-color: #E40F1C;
  color: white;
}

<template>
<div class="mine">
	<section class="user-info">
		<div class="header-bar">
			<router-link to="/home" class="goback" @click.native="goHome()"><img src="../../static/img/mine/goBack.png" alt=""></router-link>
		</div>
        <img src="//img02.hua.com/m/member/center/backgroundv3.png" alt="bg" width="100%">
        <div class="user-box">
            <div class="no-login">
                <p>Hi,欢迎来到鲜花速递网</p>
                <a href="#" class="login-btn">登录/注册</a>
            </div>
        </div>
    </section>
    <div class="top-bar clearfix">
	    <ul>
	        <li id="dfk">
		        <a href="#">
			        <img src="//img02.hua.com/m/member/center/iconPcObligation@2x.png" alt="">
			        <p>待付款</p>
		        </a>
	        </li>
	        <li id="jrps">
		        <a href="#">
			        <img src="//img02.hua.com/m/member/center/iconPcExpress@2x.png" alt="">
			        <p>今日配送</p>
		        </a>
	        </li>
	        <li id="dpj">
		        <a href="#">
			        <img src="//img02.hua.com/m/member/center/iconPcEvaluate@2x.png" alt="">
			        <p>待评价</p>
		        </a>
	        </li>
	        <li>
		        <a href="#">
			        <img src="//img02.hua.com/m/member/center/iconPcAllOrder@2x.png" alt="">
			        <p>全部订单</p>
		        </a>
	        </li>
	    </ul>
    </div>
    <div class="link-box clearfix" style="margin-top: 8px;">
	    <ul>
	        <li>
	            <a href="#">
		            <img src="//img02.hua.com/m/member/center/iconPcTicket@2x.png">
		            <p>优惠券</p>
	            </a>
	        </li>
	        <li>
	            <a href="#">
		            <img src="//img02.hua.com/m/member/center/iconPcIntegral@2x.png">
		            <p>积分</p>
	            </a>
	        </li>
	        <li>
	            <a href="#">
		            <img src="//img02.hua.com/m/member/center/iconClock@2x.png">
		            <p>生日/纪念日<br>提醒</p>
	            </a>
	        </li>
	        <li>
	            <a href="#">
		            <img src="//img02.hua.com/m/member/center/iconCollectDefault@2x.png">
		            <p>我的收藏</p>
	            </a>
	        </li>
	        <li>
	            <a href="#">
		            <img src="//img02.hua.com/m/member/center/iconPcPay@2x.png">
		            <p>在线付款</p>
	            </a>
	        </li>
	        <li>
	            <a href="#">
		            <img src="//img02.hua.com/m/member/center/bottomIconSeviceDefault@2x.png">
		            <p>联系客服</p>
	            </a>
	        </li>
	        <li>
	            <a href="#">
		            <img src="//img02.hua.com/m/member/center/iconHelp@2x.png">
		            <p>帮助</p>
	            </a>
	        </li>
	        <li>
	            <a href="#">
		            <img src="//img02.hua.com/m/member/center/iconAbout@2x.png">
		            <p>关于花礼</p
	            ></a>
	        </li>
	        
	    </ul>
    </div>
    <div class="account">
	    <span>账户管理</span>
	    <a href="/Member/AccountSetting/AccountManage">
	        <p>管理收货地址等</p>
	    </a>
    </div>

</div>
</template>

<script>
export default {
  name: 'hello', 
  data () {
    return {}
  },
  mounted(){
  		var sc=$(document);//得到document文档对象。
		$(window).scroll(function () {
			if(sc.scrollTop()>=300){
				$(".big-header").fadeIn(); 
			}
			else{
   				$(".big-header").fadeOut();
    		}
        })
  },
  methods:{
  	goHome(){
	   		this.$router.push('/home');
	   		$('a').removeClass('is-selected');
	   		$(".active_mine img").attr("src","//img02.hua.com/m/icon/my_icon_new.png");
	   		$(".active_home").addClass('is-selected');
	   		$(".active_home img").attr("src","//img02.hua.com/m/icon/home_icon_click_new.png");
	   	}
    }
}
</script>
<style>
.mine{
	background: #F0EFED;
}
.user-info {
    width: 100%;
    max-width: 750px;
    margin: 0 auto;
    position: relative;
}
.header-bar {
    position: absolute;
    top: 0px;
    height: 44px;
    width: 100%;
}
.header-bar .goback {
    display: inline-block;
    padding: 10px 5px 5px 14px;
    position: absolute;
    left: 0;
}
.header-bar .goback img {
    width: 24px;
    height: 24px;
}
.user-info .user-box {
    position: absolute;
    top: 33px;
    left: 0;
    width: 100%;
    height: 60px;
    text-align: center;
}
.no-login {
    color: #fff;
    margin-top: 5px;
    font-size: 14px;
}
.login-btn {
    padding: 0;
    height: 24px;
    line-height: 24px;
    width: 100px;
    border-radius: 12px;
    letter-spacing: 2px;
    display: inline-block;
    background: #fe6600;
    color: #fff;
    font-size: 14px;
    margin-top: 5px;
}
.top-bar {
    background-color: #fff;
    width: 100%;
    max-width: 750px;
    margin: 0 auto;
    clear: both;
    margin-bottom: 1px;
}
.top-bar ul > li {
    width: 25%;
    float: left;
    padding: 15px 0;
    text-align: center;
    position: relative;
    box-sizing: border-box;
}
.top-bar ul > li img {
    width: 32px;
}
.top-bar ul > li p {
    font-size: 11px;
    line-height: 12px;
}
.link-box {
    background: #fff;
    width: 100%;
    max-width: 750px;
    margin: 0 auto;
}
.link-box ul > li {
    float: left;
    width: 25%;
    text-align: center;
    height: 93px;
}
.link-box li:nth-child(1), .link-box li:nth-child(2), .link-box li:nth-child(3), .link-box li:nth-child(4) {
    border-bottom: 1px solid #eee;
}
.link-box li:nth-child(1), .link-box li:nth-child(2), .link-box li:nth-child(3), .link-box li:nth-child(5), .link-box li:nth-child(6), .link-box li:nth-child(7) {
    border-right: 1px solid #eee;
}
.link-box ul > li img {
    width: 32px;
    margin-top: 20px;
}
.link-box ul > li p {
    font-size: 11px;
    line-height: 20px;
    padding-bottom: 4px;
}
.account {
    width: 100%;
    max-width: 640px;
    margin: 0 auto;
    height: 40px;
    line-height: 40px;
    background: #fff;
    padding: 0 16px;
    margin-top: 10px;
}
.account span {
    font-size: 14px;
    font-weight: 500;
    float: left;
}
.account a {
    float: right;
}
.account a p {
    font-size: 11px;
    padding-right: 15px;
    background: url(//img02.hua.com/m/member/center/chevronRight@2x.png) no-repeat right center;
    background-size: 12px 12px;
}
</style>
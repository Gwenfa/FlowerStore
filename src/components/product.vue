<template>
	<div class="product">

		<div class="head_bar" style="background: rgba(255, 255, 255, 0);">
            <div class="head_bar_box">
	            <router-link to="/home" class="goback">
	                <img src="//img02.hua.com/m/icon/headChevronLeft.png" alt="" style="background: rgba(255, 255, 255, 0.5);">
	            </router-link>
	            <router-link to="/home" class="gohome">
	                <img src="//img02.hua.com/m/pro_detail/backhome.png" alt="" style="background: rgba(255, 255, 255, 0.5);">
	            </router-link>
            </div>
        </div>
        <div class="main_pro_banner">
	        <div class="swiper-container swiper-container-horizontal">
	            <div class="swiper-wrapper">
	                <div class="swiper-slide gundimg swiper-slide-active" style="width: 375px;">
	                    <img src="//img01.hua.com/uploadpic/newpic/9010011.jpg" class="swiper-lazy swiper-lazy-loaded">
	                </div>
	                <div class="swiper-slide gundimg swiper-slide-next" style="width: 375px;">
	                    <img src="//img01.hua.com/uploadpic/newpic/201709151725388540.jpg" class="swiper-lazy">
	                </div>
	                <div class="swiper-slide gundimg" style="width: 375px;">
	                    <img src="//img01.hua.com/uploadpic/newpic/201709011117442888.jpg" class="swiper-lazy">
	                </div>
	                <div class="swiper-slide gundimg" style="width: 375px;">
	                    <img src="//img01.hua.com/uploadpic/newpic/201709151725463208.jpg" class="swiper-lazy">
	                </div>
				</div>
	            <div class="swiper-pagination swiper-pagination-clickable">
		            <span class="swiper-pagination-bullet swiper-pagination-bullet-active"></span>
		            <span class="swiper-pagination-bullet"></span>
		            <span class="swiper-pagination-bullet"></span>
		            <span class="swiper-pagination-bullet"></span>
	            </div>
	        </div>
        </div>
        <div class="main_pro_text">
	        <div class="info_box">
	            <div class="collect_box">
	                <a href="javascript:DoGuanZhu(9010011,1);" id="GuanZhu">
	                    <img src="//img02.hua.com/m/pro_detail/icon_collect.png" alt="">
	                </a>
	            </div>
	            <p class="info_title">一心一意 - 玫瑰11枝，粉色勿忘我0.3扎<span class="cuxiao_tip">畅销款特价</span></p>
	            <div class="price_part">
	                <span class="now_price" id="nowPirce">￥136</span>
	                <del class="before_price" id="beforePrice">￥186</del>
	                <span class="discount_price" id="jrDiscount" style="">7.3折</span>
	            </div>
	        </div>
	        <div class="info_huayu_box" style="padding-top:12px;">
	            <span style="float:left">花语</span>
	            <p class="info_huayu">11枝玫瑰，寓意一心一意！<br>有情之人，天天是节。一句寒暖，一线相喧；一句叮咛，一笺相传；一份相思，一心相盼；一份爱意，一生相恋。</p>
	        </div>
	        <div class="info_huayu_box">
	            <span style="float:left">材料</span>
				<p class="info_huayu cailiao">红玫瑰11枝，粉色(或者紫色）勿忘我0.3扎，栀子叶适量搭配 内层白色雾面纸，外层牛皮纸,咖啡色花结</p>
	        </div>
	        <div class="info_huayu_box">
	            <span class="info_huayu_tip">配送</span>
	            <div class="info_huayu deliver_country_box">全国</div>
	        </div>
	        <div class="info_huayu_box">
	            <span class="info_huayu_tip">附送</span>
	            <p class="info_huayu">下单填写留言，即免费赠送精美贺卡！</p>
	        </div>
	        <div class="info_huayu_box">
	            <span style="float:left">说明</span>
	            <p class="info_huayu">畅销款特惠</p>
	        </div>
		</div>
		<div class="deliver_date_area">
	        <div class="time_date_box">
	            <div class="open_app_box">
	                <div class="open_app_arrow">
	                    <p class="oppen_app" id="downApp" style="" onclick="GotoApp();">App下单再减3元，立即打开</p>
	                </div>
	            </div>
	        </div>
        </div>
        <div class="advice">
	        <p class="advice_title">订单评价<a href="/comments/9010011.html" class="advice_arrow">3442条评价</a></p>
	        <div class="advice_list">
                <ul>
                    <li>
                        <img class="head_img" src="//img01.hua.com/uploadpic/newpic/9010011.jpg_80x87.jpg">
                        <div class="star_img">
                            <img src="//img02.hua.com/m/pro_detail/star5.png" alt="">
                            <p>2018-1-5</p>
                        </div>
                        <div class="advice_text_box">
                            <p class="user_name">139****9758</p>
                            <p class="user_advice">品质很好，我的朋友非常喜欢。</p>
                            <p class="user_area">安徽安庆市宜秀区光彩商务花园*****</p>
                        </div>
                    </li>
                    <li>
                        <img class="head_img" src="//img01.hua.com/uploadpic/newpic/9010011.jpg_80x87.jpg">
                        <div class="star_img">
                            <img src="//img02.hua.com/m/pro_detail/star5.png" alt="">
                            <p>2018-1-5</p>
                        </div>
                        <div class="advice_text_box">
                            <p class="user_name">157****3096</p>
                            <p class="user_advice">送货很快！很满意！！</p>
                            <p class="user_area">湖南张家界市永定区西*****</p>
                        </div>
                    </li>
                    <li>
                        <img class="head_img" src="//img01.hua.com/uploadpic/newpic/9010011.jpg_80x87.jpg">
                        <div class="star_img">
                            <img src="//img02.hua.com/m/pro_detail/star5.png" alt="">
                            <p>2018-1-5</p>
                        </div>
                        <div class="advice_text_box">
                            <p class="user_name">183****1231</p>
                            <p class="user_advice">非常满意，辛苦了，花不错</p>
                            <p class="user_area">广西南宁市仙葫经济开发区通*****</p>
                        </div>
                    </li>

                </ul>
	        </div>
        </div>
        <div class="maidian_box">
    		<img src="//img02.hua.com/m/home/maidian.jpg?a" alt="">
		</div>
		<div class="bottom_section">
    <!-- 商品信息 -->
		    <div class="pro_detail_info">
		        <div class="tab_box">
		            <div class="img_list">
		                <div class="img_box">
			                <img class="lazyimg" src="//img01.hua.com/uploadpic/images/20170915172608547.jpg" before-src="//img01.hua.com/uploadpic/images/20170915172608547.jpg">
			                <img class="lazyimg" src="//img01.hua.com/uploadpic/images/20170901112235410.jpg" before-src="//img01.hua.com/uploadpic/images/20170901112235410.jpg">
			                <img class="lazyimg" src="//img01.hua.com/uploadpic/images/20170901112235771.jpg" before-src="//img01.hua.com/uploadpic/images/20170901112235771.jpg">
			                <img class="lazyimg" src="//img01.hua.com/uploadpic/images/20170901112236136.jpg" before-src="//img01.hua.com/uploadpic/images/20170901112236136.jpg">
			                <img class="lazyimg" src="//img01.hua.com/uploadpic/images/20170915172621520.jpg" before-src="//img01.hua.com/uploadpic/images/20170915172621520.jpg">
			                <img class="lazyimg" src="//img01.hua.com/uploadpic/images/2017090111223873.jpg" before-src="//img01.hua.com/uploadpic/images/2017090111223873.jpg">
			                <img class="lazyimg" src="//img01.hua.com/uploadpic/images/20170901112239453.jpg" before-src="//img01.hua.com/uploadpic/images/20170901112239453.jpg">
			                <img class="lazyimg" src="//img01.hua.com/uploadpic/images/20170901112240840.jpg" before-src="//img01.hua.com/uploadpic/images/20170901112240840.jpg">
			                <img class="lazyimg" src="//img01.hua.com/uploadpic/images/20170901112241221.jpg" before-src="//img01.hua.com/uploadpic/images/20170901112241221.jpg">
			                <img class="lazyimg" src="//img01.hua.com/uploadpic/images/20170901112243129.jpg" before-src="//img01.hua.com/uploadpic/images/20170901112243129.jpg">
			                <img class="lazyimg" src="//img01.hua.com/uploadpic/images/20170915172645985.jpg" before-src="//img01.hua.com/uploadpic/images/20170915172645985.jpg">
			                <img class="lazyimg" src="//img01.hua.com/uploadpic/images/20170901112248140.jpg" before-src="//img01.hua.com/uploadpic/images/20170901112248140.jpg">
			                <img class="lazyimg" src="//img01.hua.com/uploadpic/images/20170901112248820.jpg" before-src="//img01.hua.com/uploadpic/images/20170901112248820.jpg">
			                <img class="lazyimg" src="//img01.hua.com/uploadpic/images/20170915172702535.jpg" before-src="//img01.hua.com/uploadpic/images/20170915172702535.jpg">
			                <a href="/Shopping/soonbuy?pp=9010011&amp;type=">
				                <img class="lazyimg" src="//img01.hua.com/uploadpic/images/20170915172718922.jpg" before-src="//img01.hua.com/uploadpic/images/20170915172718922.jpg">
			                </a>
			                <img src="//img02.hua.com/pc/images/xianhua_cardstyle.jpg">
		                </div>
		                <div class="open_more"><span class="active">展开全部</span></div>
		            </div>
		        </div>
            </div>
        </div>
    <!-- 商品信息end -->
    	<div class="footer_cart">
			    <div class="cart_md">
			        <ul>
			            <li>
			                <a id="kefu">
			                    <i class="middle_line"></i>
			                    <img src="//img02.hua.com/m/pro_detail/icon_custom_service.png">
			                    <span>客服</span>
			                </a>
			            </li>
			            <li class="call_phone">
			                <a href="tel:400-889-8188">
			                    <i class="middle_line"></i>
			                    <img src="//img02.hua.com/m/pro_detail/icon_phone.png" alt="">
			                    <span>电话</span>
			                </a>
			            </li>
			            <li>
			                <a href="/Shopping/ShowCart" id="userCart" style="position:relative">
			                    <img src="//img02.hua.com/m/icon/bottonmIcon_CartDefault.png" alt="">
			                    <span>购物车</span>
			                    <span id="cartCount" style="display:none;"></span>
			                </a>
			            </li>
			        </ul>
			        <a href="/Shopping/soonbuy?pp=9010011" class="go_buy" id="soonBuy">立即购买</a>
			        <a href="/Shopping/AddToCart?product_code=9010011" class="add_cart" id="addCart">加入购物车</a>
			        <a href="javascript:void(0);" class="sale_out">缺货或下架</a>
			    </div>
        </div>
        <div style="" id="goTopBtn"><span></span></div>
	</div>
</template>

<script>
 import Swiper from 'swiper';
 import 'swiper/dist/css/swiper.min.css';
export default{
	mounted (){
		var swiper = new Swiper('.main_pro_banner .swiper-container',{
		        autoplay:true,  
		        speed:800,  
		        loop:true,  
		        pagination: '.swiper-pagination', 
		        paginationClickable: true,
		        paginationType : 'bullets',
		        autoplayDisableOnInteraction:false,  
		        touchMoveStopPropagation:false   
		        /*effect: 'fade'*/});  
		$(function(){
			$(".mint-tabbar").hide();
		})

		function goTopEx() {
	        var obj = document.getElementById("goTopBtn");
	        function getScrollTop() {
	            return document.documentElement.scrollTop + document.body.scrollTop;
	        }
	        function setScrollTop(value) {
	            if (document.documentElement.scrollTop) {
	                document.documentElement.scrollTop = value;
	            } else {
	                document.body.scrollTop = value;
	            }
	        }
	        window.onscroll = function () {
	            getScrollTop() > window.screen.height ? obj.style.display = "" : obj.style.display = "none";
	        }
	        obj.onclick = function () {
	            var goTop = setInterval(scrollMove, 10);
	            function scrollMove() {
	                setScrollTop(0);
	                if (getScrollTop() < 1) clearInterval(goTop);
	            }
	        }
        }

     goTopEx();

	}
}
	
</script>

<style>
.head_bar {
    position: fixed;
    top: 0px;
    width: 100%;
    height: 44px;
    z-index: 999;
    max-width: 640px;
}
.head_bar_box {
    width: 100%;
    height: 44px;
}
.head_bar .goback {
    display: inline-block;
    padding: 5px;
    float: left;
}
.head_bar .gohome {
    display: inline-block;
    padding: 5px;
    float: right;
}
.head_bar .goback img {
    padding: 4px 5px 5px 4px;
}
.head_bar .gohome img {
    padding: 4px 4px 5px 5px;
}
.head_bar .goback img, .head_bar .gohome img {
    width: 24px;
    height: 24px;
    border-radius: 50%;
    box-sizing: content-box;
}
.main_pro_banner {
    border-bottom: 1px solid #f5f5f5;
}
.gundimg img {
    max-width: 100%;
    border: 0 none;
    width: 100%;
}
.main_pro_text {
    padding-bottom: 6px;
    border-bottom: 8px solid #f5f5f5;
}
.info_box {
    padding: 12px 16px 16px;
}
.info_box {
    border-bottom: 0;
}

.info_box {
    padding-bottom: 0;
}
.collect_box {
    float: right;
}
.collect_box img {
    width: 24px;
    position: relative;
    top: -2px;
}
.info_title {
    font-size: 14px;
    color: #232323;
}
.cuxiao_tip {
    color: #f60;
    margin-left: 5px;
}
.price_part {
    margin-top: 10px;
    text-align: left;
}
.now_price {
    font-size: 20px;
    color: #f60;
    text-indent: -3px;
}
.before_price {
    font-size: 12px;
    color: #9b9b9b;
}
.discount_price {
	position: relative;
    top: -3px;
    text-align: center;
    padding: 2px 6px;
    line-height: 10px;
    height: 10px;
    box-sizing: content-box;
    display: inline-block;
    font-size: 10px;
    color: #f60;
    border: 1px solid #f60;
    border-radius: 2px;
}
.info_huayu_box {
	font-size: 12px;
	padding: 6px 16px;
    overflow: hidden;
    position: relative;
}
.info_huayu {
    padding: 0 12px 0 12px;
    margin-left: 24px;
    font-size: 12px;
    color: #9b9b9b;
    position: relative;
    text-align: justify;
}
.info_huayu_tip {
    position: absolute;
    left: 16px;
    top: 50%;
    margin-top: -8px;
}
.time_date_box {
    border-bottom: 8px solid #f5f5f5;
    text-align: left;
}
.open_app_box {
    padding: 13px 16px;
    overflow: hidden;
    line-height: 24px;
    border-bottom: 1px solid #f5f5f5;
}
.open_app_arrow {
    background: url(//img02.hua.com/m/pro_detail/arrow_right_orange.png) no-repeat right;
    background-size: 12px;
}
.oppen_app {
    font-size: 12px;
    color: #f60;
    padding-left: 20px;
    background: url(//img02.hua.com/m/pro_detail/app_download_icon.png) no-repeat left;
    background-size: 17px;
    margin-left: -3px;
}
.advice_title {
    padding: 9px 16px;
    border-bottom: 1px solid #f5f5f5;
    font-size: 12px;
    text-align: left;
}
.advice_arrow {
    float: right;
    color: #9b9b9b;
    font-size: 10px;
    padding-right: 15px;
    background: url(//img02.hua.com/m/pro_detail/arrow_right_default.png) no-repeat right;
    background-size: 12px;
}
.advice_list li {
    padding: 12px 16px;
    overflow: hidden;
}
.advice_list .head_img {
    width: 48px;
    float: left;
}
.star_img {
    width: 67px;
    float: right;
    margin-top: 8px;
}
.star_img img {
    width: 60px;
    float: right;
}
.star_img p {
    color: #9b9b9b;
    font-size: 10px;
    margin-top: 13px;
    text-align: right;
}
.advice_text_box {
    margin-left: 60px;
    width: 63%;
}
.user_name, .user_area {
    font-size: 10px;
    color: #9b9b9b;
    text-align: left;
}
.user_advice {
	font-size: 12px;
	text-align: left;
}
.maidian_box {
    border-bottom: 1px solid #f5f5f5;
    border-top: 1px solid #f5f5f5;
    height: 68px;
}
.maidian_box img {
    width: 100%;
}
.bottom_section {
    padding-bottom: 49px;
}
.tab_box {
    border-bottom: 8px solid #f5f5f5;
}
.img_list {
    position: relative;
}
.img_box img {
    width: 100%;
}
.open_more {
    display: none;
    position: absolute;
    bottom: 0px;
    text-align: center;
    height: 36px;
    line-height: 36px;
    color: #232323;
    width: 100%;
    border-top: 1px solid #f5f5f5;
    background: #fff;
}
.footer_cart {
    position: fixed;
    bottom: 0px;
    height: 49px;
    width: 100%;
    z-index: 9999;
    max-width: 640px;
}
.cart_md {
    background: #fff;
    overflow: hidden;
}
.cart_md ul {
    width: 40%;
    float: left;
    position: relative;
}
.cart_md li {
    width: 33.33%;
    text-align: center;
    font-size: 10px;
    float: left;
}
.cart_md li a {
    display: inline-block;
    width: 100%;
    height: 100%;
}
.cart_md li a span{
	display: inline-block;
}
.middle_line {
    display: inline-block;
    width: 1px;
    height: 20px;
    background-color: #999;
    transform: scale(0.5, 1);
    float: right;
    margin-top: 14px;
}
.cart_md li img {
    width: 24px;
    margin: 5px auto 0px;
}
.cart_md>a {
    display: inline-block;
    width: 30%;
    height: 49px;
    float: right;
    text-align: center;
    font-size: 14px;
    color: #fff;
    line-height: 49px;
}
.go_buy {
    background: #f60;
}
.add_cart {
    background: rgb(255, 167, 71);
}
.cart_md .sale_out {
    width: 60%;
    background: #ccc;
    display: none;
}
#goTopBtn {
    position: fixed;
    bottom: 60px;
    right: 15px;
    cursor: pointer;
    height: 36px;
    width: 36px;
    background-color: #fff;
    border-radius: 22px;
    opacity: .8;
    z-index: 999;
    border: 1px solid #999;
    box-sizing: border-box;
}
#goTopBtn span {
    display: inline-block;
    width: 24px;
    height: 24px;
    background: url(//img02.hua.com/m/icon/arrow_Top.png?a) no-repeat center;
    background-size: 24px 24px;
    margin-top: 5px;
}
</style>

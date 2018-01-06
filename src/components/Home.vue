<template>
  <div class="home">
    <div class="headerbanner">
        <div class="swiper-container" id="banner">
            <div class="swiper-wrapper">  
                <div class="swiper-slide"><img width="100%" src="../../static/img/home/banner1.jpg"></div>  
                <div class="swiper-slide"><img width="100%" src="../../static/img/home/banner2.jpg"></div>  
                <div class="swiper-slide"><img width="100%" src="../../static/img/home/banner3.png"></div>  
            </div>  
            <!-- Add Pagination -->  
            <div class="swiper-pagination"></div>
        </div> 
    </div>
    <div class="fadesearch">
         <mt-search v-model="value" cancel-text="" placeholder="搜索" @click.native="goSearch()"></mt-search>
         <div class="login"> <a href="/Passport/Login/">登录</a></div>
    </div>
    <div class="search">
         <mt-search v-model="value" cancel-text="" placeholder="搜索" @click.native="goSearch()"></mt-search>
		 <div class="login"> <a href="/Passport/Login/">登录</a></div>
    </div>
    <div class="conpany_info">
		<ul>
			<li style="width:25%">· 认证龙头企业</li>
			<li style="width:21%">· 12年品牌</li>
			<li style="width:21%">· 3小时送达</li>
			<li style="width:33%">· 最近<a style="text-decoration: underline;" href="/productpj/" id="pjCount">227700</a>条好评</li>
		</ul>
	</div>
	<div class="pro_type_box">
		<div class="pro_type">
			<ul>
				<li>
					<a href="/flower/">
						<img src="//img02.hua.com/m/icon/xianhua_icon.png" alt="鲜花">
						<p>鲜花</p>
					</a>
				</li>
				<li>
					<a href="/yongshenghua/">
						<img src="//img02.hua.com/m/icon/yongshenghua_icon.png" alt="永生花">
						<p>永生花</p>
					</a>
				</li>
				<li>
					<a href="/cake/">
						<img src="//img02.hua.com/m/icon/cake_icon.png" alt="蛋糕">
						<p>蛋糕</p>
					</a>
				</li>
				<li>
					<a href="/gifts/">
						<img src="//img02.hua.com/m/icon/gift_icon.png" alt="礼品">
						<p>礼品</p>
					</a>
				</li>
				<li>
					<a href="/gifts/chocolates/">
						<img src="//img02.hua.com/m/icon/choclate_icon.png" alt="巧克力">
						<p>巧克力</p>
					</a>
				</li>
			</ul>
		</div>
	</div>
	<div class="featured">
		<div class="title">
			<div class="title_line"></div>
			<p class="title_name">鲜花精选</p>
		</div>
	</div>
	<div class="fea_pro_list" style="border-bottom:8px solid #eee;">
		<ul>
			<li v-for="flower in flowerList">
				<div class="pro_box">
					<router-link to="/product">
						<img :src="flower.flowerimg" alt="鲜花/一心一意">
						<div class="pro_text">
							<p class="pro_name">{{flower.pro_name}}</p>
							<p class="pro_detail">{{flower.pro_detail}}</p>
							<p class="pro_price">￥{{flower.pro_price}}</p>
						</div>
					</router-link>
				</div>
			</li>
			
		</ul>
		<div>
			<a href="/flower/" class="more_btn">全部鲜花<span class="arrow_right"></span></a>
		</div>
    </div>
	<div class="business">
		<div class="business_box">
            <ul>
                <li class="active" id="btn1">
                    <img src="//img02.hua.com/m/pro_detail/brand_icon01.png" alt="行业龙头">
	                <img src="//img02.hua.com/m/pro_detail/brand_icon010.png" alt="">
	                <span>行业龙头</span>
                </li>
                <li id="btn2">
	                <img src="//img02.hua.com/m/pro_detail/brand_icon02.png" alt="品牌理念">
	                <img src="//img02.hua.com/m/pro_detail/brand_icon020.png" alt="">
	                <span>品牌理念</span>
                </li>
                <li id="btn3">
	                <img src="//img02.hua.com/m/pro_detail/brand_icon03.png" alt="3小时送达">
	                <img src="//img02.hua.com/m/pro_detail/brand_icon030.png" alt="">
	                <span>3小时送达</span>
                </li>
                <li id="btn4">
	                <img src="//img02.hua.com/m/pro_detail/brand_icon04.png" alt="送前实拍">
	                <img src="//img02.hua.com/m/pro_detail/brand_icon040.png" alt="">
	                <span>送前实拍</span>
                </li>
            </ul>
        </div>
        <div class="brand_img_box">
            <div class="swiper-container swiper-container-horizontal">
                <div class="swiper-wrapper" style="transition-duration: 0ms; transform: translate3d(-984px, 0px, 0px);">
                    <div class="swiper-slide gundimg" style="width: 328px;">
                    <img alt="行业龙头" class="swiper-lazy swiper-lazy-loaded" src="//img02.hua.com/m/pro_detail/brand001.jpg?a">
                    </div>
                    <div class="swiper-slide gundimg" style="width: 328px;">
                        <img alt="品牌理念" class="swiper-lazy shipin swiper-lazy-loaded" src="//img02.hua.com/m/pro_detail/brand002feben.jpg?">
                    </div>
                    <div class="swiper-slide gundimg swiper-slide-prev" style="width: 328px;">
                        <img alt="3小时送达" class="swiper-lazy swiper-lazy-loaded" src="//img02.hua.com/m/pro_detail/brand003.jpg?a">
                    </div>
                    <div class="swiper-slide gundimg swiper-slide-active" style="width: 328px;">
                        <img alt="送前实拍" class="swiper-lazy swiper-lazy-loaded" src="//img02.hua.com/m/pro_detail/brand004.jpg?a">
                    </div>
                </div>
                <div class="swiper-pagination swiper-pagination-clickable">
                    <span class="swiper-pagination-bullet swiper-pagination-bullet-active"></span>
                    <span class="swiper-pagination-bullet"></span>
                    <span class="swiper-pagination-bullet"></span>
                    <span class="swiper-pagination-bullet "></span>
                </div>
            </div>
        </div>
        <div class="brand_text">
            <div class="active">
                <p>专注鲜花礼品12年，2016年获评“鲜花行业龙头企业”</p>
            </div>
            <div class="">
                <p>花礼网倡导勇敢表达爱，享受爱的美好</p>
            </div>
            <div>
                <p>覆盖全国1000+城市，最快1~3小时送达</p>
            </div>
            <div>
                <p>坚持公开所有花款实拍，严格管控质量</p>
            </div>
        </div>		
	</div>
    <div class="user_box">
        <div class="login_help">
            <ul class="user_login">
                <li><a href="/huayu/">花语大全</a></li>
                <li><a href="/Ordercx/Index/">查单</a></li>
                <li><a href="/profile/about.htm">关于我们</a></li>
            </ul>
        </div>
        <div class="platform">
            <dl><dt><a href="/gomobile/" rel="nofollow"><img src="//img02.hua.com/m/icon/icon-phonenew.png" alt="mobile"></a></dt></dl>
            <dl><dt><a id="kefu" href="https://www.sobot.com/chat/h5/index.html?sysNum=d22b0bfa87fd42258397365c95bc5e08&amp;partnerId=0"><img src="//img02.hua.com/m/icon/icon-kefu.png" alt="客服"></a></dt></dl>
        </div>
        <div class="copyright">Copyright © 2005~2017 花礼网(中国鲜花礼品网) 版权所有<br>中国鲜花网领先品牌，鲜花速递专家！</div>
    </div>
    <div id="goTopBtn" style=""> <span></span></div>
    <div class="kefu_shouye"><span></span></div>
<div style="height:55px"></div>
  </div>
</template>

<script>
 import Swiper from 'swiper';
 import 'swiper/dist/css/swiper.min.css';
import {api} from '@/global/api'

export default {
  name: 'hello', 
  data () {
    return {
        value:null,
      msg: 'Welcome to Your Vue.js App',
      listImg: ["//img02.hua.com/slider/17_banner_d11_m.jpg","//img02.hua.com/slider/17_banner_tx_m.jpg","//img02.hua.com/slider/new_banner_yongganai.png"],
      flowerList:null
  }
},
  mounted() {
  	var vm=this;
    vm.getaData();
    vm.box_Click();
    var sc=$(document);//得到document文档对象。
        $(window).scroll(function () {
            if(sc.scrollTop()>0){
                $(".fadesearch").fadeIn(); 
            }
            else{
                $(".fadesearch").fadeOut();
            }
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

  	var swiper = new Swiper('.headerbanner .swiper-container',{
        autoplay:true,  
        speed:1000,  
        loop:true,  
        pagination: '.swiper-pagination', 
        paginationClickable: true,
        paginationType : 'bullets',
        autoplayDisableOnInteraction:false,  
        touchMoveStopPropagation:false   
        /*effect: 'fade'*/});  
        },
    methods:{
	   	getaData(){
	      this.$http.get(api.HomeData).then(function(response){
	        this.flowerList=response.data.flowerlist;
	        console.log("-----flowerList",this.flowerList)
	        console.log("-----response",response);
	      })
	    },
	   	goSearch(){
	   		this.$router.push('/classify');
	   		$('a').removeClass('is-selected');
	   		$(".active_home img").attr("src","//img02.hua.com/m/icon/home_icon_new.png");
	   		$(".active_classify").addClass('is-selected');
	   		$(".active_classify img").attr("src","//img02.hua.com/m/icon/classify_icon_click_new.png");
	   	},
	   	box_Click(){
        var brand = new Swiper('.brand_img_box .swiper-container', {
            pagination: '.brand_img_box .swiper-pagination',
            slidesPerView: 1,
            paginationClickable: true,
            spaceBetween: 0,
            autoplay: 0,
            loop: false,
            autoplayDisableOnInteraction: false,
            lazyLoading: true,
            onSlideChangeEnd:function(swiper){
                console.log(swiper.activeIndex);
                $('.business_box li').eq(swiper.activeIndex).addClass('active').siblings().removeClass('active');
                $('.brand_text div').eq(swiper.activeIndex).addClass('active').siblings().removeClass('active');
            }
        });

        $('#btn1').click(function(){
            brand.slideTo(0, 1000, false);
            $(this).addClass('active').siblings().removeClass('active');
            $('.brand_text div').eq($(this).index()).addClass('active').siblings().removeClass('active');
        });
        $('#btn2').click(function(){
            brand.slideTo(1, 1000, false);
            $(this).addClass('active').siblings().removeClass('active');
            $('.brand_text div').eq($(this).index()).addClass('active').siblings().removeClass('active');
        });
        $('#btn3').click(function(){
            brand.slideTo(2, 1000, false);
            $(this).addClass('active').siblings().removeClass('active');
            $('.brand_text div').eq($(this).index()).addClass('active').siblings().removeClass('active');
        });
        $('#btn4').click(function(){
            brand.slideTo(3, 1000, false);
            $(this).addClass('active').siblings().removeClass('active');
            $('.brand_text div').eq($(this).index()).addClass('active').siblings().removeClass('active');
        });

	  //  		$(".business_box li").click(function () {
	  //  			// alert("hello")
			// 	$(".business_box li").removeClass("active").eq($(this).index()).addClass("active");
			// });
	   	}
   }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.home .swiper-container {
    height: 8.5rem;
}
.home .fadesearch {
    width: 100%;
    height: 42px;
    position: fixed;
    z-index: 9999;
    top: 0;
    background: white;
    display: none;
}
.home .fadesearch .mint-search input,.home .fadesearch .mint-search .mint-searchbar .mint-searchbar-inner{
    background: #f5f5f5;
}
.home .search{
    width: 100%;
    height: 42px;
    position: absolute;
    top: 0;
    background: white;
}

.home .mint-search {
	position: absolute;
    top: 7px;
    right: 50px;
    height: auto;
    width: 8.3rem;
}

.mint-search-list {
	display: none;
}
.home .mint-search .mint-searchbar {
    background:none;
    padding: 0;
}
.home .mint-searchbar-inner{
	border-radius: 5px;
	width: 165px;
}
.login{
	position: absolute;
    top: 15px;
    z-index: 999;
    font-size: 12px;
    right: 12px;
}
.conpany_info {
    border-bottom: 1px solid #eee;
}
.conpany_info ul {
    font-size: 0.5rem;
    overflow: hidden;
    height: 28px;
    line-height: 28px;
}
.conpany_info ul li {
    float: left;
    color: #9b9b9b;
    text-align: center;
}
.pro_type {
    padding: 7px 3px 8px 3px;
    border-bottom: 8px solid #eee;
}
ul {
    overflow: hidden;
}
.pro_type ul li {
    float: left;
    width: 20%;
    text-align: center;
}
.pro_type ul li img {
    width: 48px;
    display: block;
    margin: 0 auto;
}
.pro_type ul li p {
    font-size: 11px;
    margin-top: 3px;
}
.featured {
    overflow: hidden;
}
.featured .title .title_line {
    width: 160px;
    height: 1px;
    background-color: #bbb;
    margin: 22px auto 0;
}
.title .title_name {
    width: 90px;
    text-align: center;
    background-color: #fff;
    font-size: 16px;
    color: #222;
    margin: -12px auto 13px;
}
.fea_pro_list {
    padding: 0 0 0 8px;
    overflow: hidden;
    padding-bottom: 18px;
}
.fea_pro_list li {
    float: left;
    width: 50%;
    padding-right: 8px;
    padding-bottom: 8px;
}
.fea_pro_list .pro_box {
    border: 1px solid;
    border-color: #efefef;
    position: relative;
}
.fea_pro_list .pro_box img {
    width: 100%;
    padding: 3px;
    height: 7.94rem;
    max-height: 317px;
}
.fea_pro_list .pro_box .pro_text {
    padding: 6px;
}
.fea_pro_list .pro_box .pro_name {
    font-size: 12px;
    color: #232323;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
}
.fea_pro_list .pro_box .pro_detail {
    color: #777;
    font-size: 10px;
    line-height: 13px;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
}
.fea_pro_list .pro_box .pro_price {
    color: #222;
    font-size: 12px;
}
.fea_pro_list .more_btn {
    display: block;
    width: 119px;
    margin: 0 auto;
    height: 34px;
    line-height: 32px;
    font-size: 12px;
    border: 1px solid #ddd;
    border-radius: 2px;
    text-align: center;
    margin-top: 5px;
    color: #777;
}
.arrow_right {
    display: inline-block;
    width: 12px;
    height: 12px;
    background: url(//img02.hua.com/m/icon/chevron_Right.png) no-repeat center;
    background-size: 24px 24px;
    position: relative;
    top: 2px;
    opacity: .7;
}
.business {
    border-bottom: 8px solid #f5f5f5;
    height: 93vw;
    max-height: 470px;
}
.business_box ul {
    padding: 12px 3% 14px;
}
.business_box li.active {
    color: #fe6600;
}
.business_box li {
    float: left;
    width: 25%;
    text-align: center;
    color: #9b9b9b;
    font-size: 12px;
}
.business_box li img {
    width: 48px;
    margin: 0 auto;
    margin-bottom: 5px;
}
.business_box li img:nth-child(1) {
    display: block;
}
.business_box li img:nth-child(2) {
    display: none;
}
.business_box li.active img:first-child {
    display: none;
}
.business_box li.active img:nth-child(2) {
    display: block;
}
.brand_img_box {
    padding: 2px 16px 0 16px;
}
.swiper-container {
    margin: 0 auto;
    position: relative;
    overflow: hidden;
    z-index: 1;
    background: #fff;
}
.business .swiper-pagination {
    bottom: 18px;
}
.swiper-container-horizontal>.swiper-pagination .swiper-pagination-bullet {
    margin: 0 5px;
}
.swiper-pagination-bullet {
    background-color: transparent;
    border: 1px solid #fff;
}
.swiper-pagination-bullet {
    width: 7px;
    height: 7px;
    display: inline-block;
    border-radius: 100%;
    background: #fff;
    opacity: .9;
}
.swiper-pagination-bullet-active {
    opacity: 1;
    background: #f60;
}
.business .brand_text {
    padding: 5px 16px!important;
    line-height: 16px!important;
    font-weight: 700!important;
    text-align: center;
    line-height: 23px!important;
}
.business .brand_text div {
    display: none;
}
.business .brand_text div.active {
    display: block;
}
.business .brand_text p {
    font-size: 12px;
    color: #232323;
    font-weight: 400;
    line-height: 18px;
    margin-bottom: 8px;
}
.login_help {
    border-bottom: 1px solid #eee;
    padding-top: 16px;
}
.login_help ul {
    margin-bottom: 16px;
    overflow: hidden;
}
.login_help ul li {
    float: left;
    text-align: center;
    font-size: 12px;
    width: 33.3%;
}
.login_help .user_login li a {
    background-color: #eee;
    color: #444;
    border-radius: 2px;
}
.platform {
    overflow: hidden;
    padding: 16px 10% 14px 10%;
    color: #777;
    font-size: 12px;
    border-bottom: 1px solid #eee;
}
.platform dl {
    float: left;
    width: 50%;
    text-align: center;
}
.login_help ul li a {
    display: inline-block;
    padding: 4px 19px;
}
.platform dl a {
    display: inline-block;
    width: 36px;
}
.platform dl img {
    display: inline-block;
    width: 36px;
    margin: 5px 0 8px 0;
}
.copyright {
    font-size: 10px;
    text-align: center;
    color: #ccc;
    padding: 16px 0;
}
#goTopBtn {
    position: fixed;
    bottom: 120px;
    right: 15px;
    cursor: pointer;
    height: 36px;
    width: 36px;
    background-color: #fff;
    border-radius: 22px;
    opacity: .8;
    z-index: 999;
    border: 1px solid #999;
}
#goTopBtn span {
    display: inline-block;
    width: 24px;
    height: 24px;
    background: url(//img02.hua.com/m/icon/arrow_Top.png?a) no-repeat center;
    background-size: 24px 24px;
    margin-top: 5px;
}
.kefu_shouye {
    position: fixed;
    bottom: 70px;
    right: 15px;
    cursor: pointer;
    height: 36px;
    width: 36px;
    background-color: #fff;
    border-radius: 22px;
    opacity: .8;
    z-index: 999;
    border: 1px solid #999;
}
.kefu_shouye span {
    display: inline-block;
    width: 24px;
    height: 24px;
    background: url(//img02.hua.com/m/member/kefu_shouye.png) no-repeat center;
    background-size: 24px 24px;
    margin-top: 5px;
}
</style>

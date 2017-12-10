<template>
<div class="Shoping_Cart">
	<div class="header" style="background:rgba(250,250,250,0.9);height:44px;border-bottom: 1px solid #e4e4e4;">
        <div class="header-btn_fh fl">
            <router-link to="/home" style="padding-top:11px;height:auto;">
	            <span style="height:24px;width:24px;background:none;">
	            	<img src="//img02.hua.com/m/icon/headChevronLeft.png" alt="" style="width:24px;height:24px;float: left;margin-left:12px;">
	            </span>
            </router-link>
        </div>
        <div class="logo" style="height:44px;line-height:44px;color:#232323">购物车</div>
    </div>
    <div class="content">
	    <div style="position:relative;text-align:center;">
	            <img src="//img02.hua.com/m/empty_cart2.png" width="60%" style="max-width:512px;" class="img">
	        <a href="/">
	            <p style="position:absolute;left:38%;top:84%;color:#f60;background:#fff;padding: 0 20px;border-radius:3px;height:32px;line-height:32px;border:1px solid #f60;font-size:14px;">去逛逛</p>
	        </a>
	        <p class="cart_text">这里什么都没有啊～</p>
	    </div>
        <div class="cake_lb"><font style="color:#111;font-size:14px;">为你推荐hh</font></div>
	        <div class="main">
	            <ul class="activity-list tuijian_ul" style="width: 504px;">
					<li class="activity-item tuijian_list">
                        <a href="/product/9012239.html">
                            <img src="//img01.hua.com/uploadpic/newpic/9012239.jpg_220x240.jpg" class="activity-img">
                            <font class="price">￥392</font>
                        </a>
                    </li>
                    <li class="activity-item tuijian_list">
                        <a href="/product/9012247.html">
                            <img src="//img01.hua.com/uploadpic/newpic/9012247.jpg_220x240.jpg" class="activity-img">
                            <font class="price">￥339</font>
                        </a>
                    </li>
                    <li class="activity-item tuijian_list">
                        <a href="/product/9012246.html">
                            <img src="//img01.hua.com/uploadpic/newpic/9012246.jpg_220x240.jpg" class="activity-img">
                            <font class="price">￥296</font>
                        </a>
                    </li>
                    <li class="activity-item tuijian_list">
                        <a href="/product/9010011.html">
                            <img src="//img01.hua.com/uploadpic/newpic/9010011.jpg_220x240.jpg" class="activity-img">
                            <font class="price">￥126</font>
                        </a>
                    </li>
                    <li class="activity-item tuijian_list">
                        <a href="/product/9012011.html">
                            <img src="//img01.hua.com/uploadpic/newpic/9012011.jpg_220x240.jpg" class="activity-img">
                            <font class="price">￥218</font>
                        </a>
                    </li>
                    <li class="activity-item tuijian_list">
                        <a href="/product/9010966.html">
                            <img src="//img01.hua.com/uploadpic/newpic/9010966.jpg_220x240.jpg" class="activity-img">
                            <font class="price">￥235</font>
                        </a>
                    </li>
	            </ul>
	        </div>
    </div>
</div>
</template>
<script>
export default {
  data () {
    return {}
},
  mounted() {
  	$(function () {
            var num = $('.tuijian_list').length;
            var ulWidth = num * 84;
            console.log(num);
            $('.tuijian_ul').width(ulWidth);
        })
  }
}

</script>

<style>
.header-btn_fh a {
    display: block;
    padding: 7px 0 0 0;
    height: 34px;
}
.fl {
    float: left;
}
.header .logo {
    margin: 0 auto;
    text-align: center;
    width: 50%;
    cursor: pointer;
    font-size: 17px;
}
.content .img {
    margin: 30px 0 10px 0;
}
.cart_text {
    font-size: 14px;
    text-align: center;
    color: rgb(75,75,75);
    padding-bottom: 70px;
}
.cake_lb {
    clear: both;
    color: #666666;
    line-height: 38px;
    border-top: 8px solid #eee;
    padding: 0 10px;
    padding-left: 16px!important;
    border-bottom: none!important;
}
.main {
    width: 100%;
    margin: 0 auto;
    max-width: 640px;
    font-size: 14px;
}
.activity-list {
    padding: 0px 0px 0px 8px;
    overflow: hidden;
}
.activity-item {
	float: left;
    margin-top: 0!important;
    width: 84px!important;
    text-align: center;
}
.activity-list li a {
    display: block;
    width: auto;
    padding: 0px;
    margin: 0px 8px 0px 0px;
    -webkit-border-radius: 1px;
    -moz-border-radius: 1px;
    border-radius: 1px;
}
.activity-item img {
    width: 100%;
    height: auto;
    margin-top: 12px!important;
}
</style>
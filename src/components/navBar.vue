<template>
    <div class="page" id="homePage">
        
        <!-- 这里是页面内容区 -->
        <div class="content" id="contentBox">
            <div class="placeholder-header"></div>
            <nav class="nav-fixed" id="navFixed" scroll="0" ref="navFixed">
                <ul class="nav-ul content" id="navUl">
                    <li v-for="(item,index) in navList" :class="{'active': item.key}" :key="index" :val="index">
                        {{item.val}}
                    </li>
                </ul>
            </nav>
            <div class="content-block tax-content">
                <div class="content-scroll">
                    <div class="search">
                        <div class="search-icon">
                            <i class="iconfont icon-saomiao"></i>
                        </div>
                        <div class="search-input">
                            <input type="text" placeholder="请输入您需要搜索的功能">
                            <i class="iconfont icon-tubiao11"></i>
                        </div>
                    </div>

                    <div class="menu-box">
                        <div class="menu-wrap" ref="menu-wrap">
                            <div class="menu-item personal-tax">
                                <h4>
                                    <span>个</span>人所得税</h4>
                                <ul class="item-ul">
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_1.png')" alt="">
                                            <span>个人所得税查询</span>
                                        </div>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_2.png')" alt="">
                                            <span>自行申报A表无扣款义务人</span>
                                        </div>
                                    </li>
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_3.png')" alt="">
                                            <span>自行申报A表两处以上所得</span>
                                        </div>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_4.png')" alt="">
                                            <span>自行申报B表境外所得</span>
                                        </div>
                                    </li>
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_5.png')" alt="">
                                            <span>年所得12万以上</span>
                                        </div>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_6.png')" alt="">
                                            <span>生产经营A表月季</span>
                                        </div>
                                    </li>
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_7.png')" alt="">
                                            <span>生产经营B表年度</span>
                                        </div>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_8.png')" alt="">
                                            <span>生产经营C表两个或以上</span>
                                        </div>
                                    </li>
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_9.png')" alt="">
                                            <span>完税证明邮寄</span>
                                        </div>
                                        <div>

                                        </div>
                                    </li>
                                </ul>
                            </div>
                            <div class="menu-item personal-tax">
                                <h4>
                                    <span>社</span>保费</h4>
                                <ul class="item-ul">
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_10.png')" alt="">
                                            <span>社保费查询</span>
                                        </div>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_11.png')" alt="">
                                            <span>社保业务</span>
                                        </div>
                                    </li>
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_12.png')" alt="">
                                            <span>托收单清缴</span>
                                        </div>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_13.png')" alt="">
                                            <span>缴费登记</span>
                                        </div>
                                    </li>
                                </ul>
                            </div>
                            <div class="menu-item personal-tax">
                                <h4>
                                    <span>车</span>船税</h4>
                                <ul class="item-ul">
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_14.png')" alt="">
                                            <span>车船税查询</span>
                                        </div>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_15.png')" alt="">
                                            <span>车船税缴款</span>
                                        </div>
                                    </li>
                                </ul>
                            </div>
                            <div class="menu-item personal-tax">
                                <h4>
                                    <span>房</span>产交易</h4>
                                <ul class="item-ul">
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_16.png')" alt="">
                                            <span>契税查询</span>
                                        </div>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_17.png')" alt="">
                                            <span>房产税交易智能办税</span>
                                        </div>
                                    </li>
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_18.png')" alt="">
                                            <span>二手房交易</span>
                                        </div>
                                        <div>

                                        </div>
                                    </li>
                                </ul>
                            </div>
                            <div class="menu-item personal-tax">
                                <h4>
                                    <span>缴</span>款</h4>
                                <ul class="item-ul">
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_19.png')" alt="">
                                            <span>税费缴款</span>
                                        </div>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_20.png')" alt="">
                                            <span>申报作废</span>
                                        </div>
                                    </li>
                                </ul>
                            </div>
                            <div class="menu-item personal-tax">
                                <h4>
                                    <span>完</span>税证明</h4>
                                <ul class="item-ul">
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_21.png')" alt="">
                                            <span>电子税票</span>
                                        </div>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_22.png')" alt="">
                                            <span>证明查验</span>
                                        </div>
                                    </li>
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_23.png')" alt="">
                                            <span>文书查验</span>
                                        </div>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_24.png')" alt="">
                                            <span>个人完税查验</span>
                                        </div>
                                    </li>
                                </ul>
                            </div>
                            <div class="menu-item personal-tax">
                                <h4>
                                    <span>住</span>房公积金</h4>
                                <ul class="item-ul">
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_21.png')" alt="">
                                            <span>总额查询</span>
                                        </div>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_22.png')" alt="">
                                            <span>明细查询</span>
                                        </div>
                                    </li>
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_23.png')" alt="">
                                            <span>提取申请</span>
                                        </div>
                                        <div>

                                        </div>
                                    </li>
                                </ul>
                            </div>
                            <div class="menu-item personal-tax">
                                <h4>
                                    <span>医</span>疗</h4>
                                <ul class="item-ul">
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_21.png')" alt="">
                                            <span>问医生</span>
                                        </div>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_22.png')" alt="">
                                            <span>智能预诊</span>
                                        </div>
                                    </li>
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_23.png')" alt="">
                                            <span>体检预约</span>
                                        </div>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_21.png')" alt="">
                                            <span>儿科诊所</span>
                                        </div>
                                    </li>
                                </ul>
                            </div>
                            <div class="menu-item personal-tax">
                                <h4>
                                    <span>交</span>通情况</h4>
                                <ul class="item-ul">
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_19.png')" alt="">
                                            <span>地铁购票</span>
                                        </div>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_20.png')" alt="">
                                            <span>羊城通乘车码</span>
                                        </div>
                                    </li>
                                </ul>
                            </div>
                            <div class="menu-item personal-tax">
                                <h4>
                                    <span>政</span>务</h4>
                                <ul class="item-ul">
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_21.png')" alt="">
                                            <span>港澳台签证办理</span>
                                        </div>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_22.png')" alt="">
                                            <span>12315</span>
                                        </div>
                                    </li>
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_23.png')" alt="">
                                            <span>法律服务</span>
                                        </div>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_24.png')" alt="">
                                            <span>广州来穗通</span>
                                        </div>
                                    </li>
                                </ul>
                            </div>
                            <div class="menu-item personal-tax">
                                <h4>
                                    <span>综</span>合应用</h4>
                                <ul class="item-ul">
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_21.png')" alt="">
                                            <span>证件照拍照</span>
                                        </div>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_22.png')" alt="">
                                            <span>司法拍卖</span>
                                        </div>
                                    </li>
                                    <li>
                                        <div>
                                            <img :src="require('assets/images/taxes/tax_23.png')" alt="">
                                            <span>境外游</span>
                                        </div>
                                        <div>
                            
                                        </div>
                                    </li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import BScroll from 'better-scroll'

export default {
    data(){
       return {
           navList: [
                {key: true, val:'个人所得税'},
                {key: false, val:'社保费'},
                {key: false, val:'车船税'},
                {key: false, val:'房产交易'},
                {key: false, val:'缴款'},
                {key: false, val:'完税证明'},
                {key: false, val: '住房公积金'},
                {key: false, val: '医疗'},
                {key: false, val: '交通情况'},
                {key: false, val: '政务'},
                {key: false, val:'综合应用'},
            ],
            navScroll: '',   //导航滚动实例
            menuScroll: '',  //菜单列表滚动实例
            liNum: 0,      //记录当前屏幕宽度下正常展示导航条的li的个数
            menuItemTop: [],     //记录每个菜单的offsetTop值
            liDisX: 0,    //li每次滑动距离
            clickFlag: false,   //控制在点击导航栏时就禁用滚动事件中触发的导航栏滑动
            navLiLeft: [],    //记录导航栏每个li的offsetLeft值
            navLiActive: 0,   //记录当前导航菜单激活的索引值

            controlOnce: true,  //控制展示导航栏函数只执行一次

            navLeftFlag: false,   //控制导航栏左向滚动时机
            navRightFlag: false,  //控制导航栏右向滚动时机
       }
    },

    methods: {
        //获取原生元素的css属性值
        getStyle(obj, attr){
            return obj.currentStyle[attr] || window.getComputedStyle(obj, attr);
        },

        //点击切换导航栏li
        changeNavList (options) {  
            var that = this;
            var hosEl = document.querySelector(options.hosEl);
            var navUl = hosEl.children[0];
            // 需要使用原生的click事件 
            navUl.onclick = function (e) {
                var e = event||window.event;
                if (e.stopPropagation) {
                    e.stopPropagation();
                } else {
                    e.cancelBubble = true;
                }
                
                //当在执行点击导航栏li时就禁用内容滚动区域导致的导航栏滑动事件
                that.clickFlag = true;
                var index = e.target.getAttribute('val');
                that.navList.forEach((ele,num) => {
                    ele.key = false;
                    if (index == num) {
                        ele.key = true;
                    }
                });

                var windowWidth = window.innerWidth/2;
                var ulWidth = navUl.innerWidth;
                var disX = ulWidth - window.innerWidth;
                if (e.clientX > windowWidth) {
                    if (that.navScroll.x > that.navScroll.maxScrollX) {
                        if (that.liNum == 0) {
                            //当屏幕较宽导致导航栏最后一个li不完全展示时，此时that.liNum的值为0，
                            // 点击滑动时滑动距离需要使用导航条的宽度减去屏幕宽度值
                            that.navScroll.scrollBy(-disX, 0, 100);
                        }else{
                            that.navScroll.scrollBy(-that.liDisX, 0, 100);
                        }
                    }
                }else{
                    if (that.navScroll.x < 0) {
                        if (that.liNum == 0) {
                            that.navScroll.scrollBy(disX, 0, 100);
                        }else{
                            that.navScroll.scrollBy(that.liDisX, 0, 100);
                        }
                    }
                }

                that.menuItemTop.forEach((ele,num)=>{
                    if (index == num) {
                        that.menuScroll.scrollTo(0, -that.menuItemTop[num],200);
                    }
                })
            }
        },


        //顶部导航栏显示函数及相关事件处理
        showUl(options){ 
            var that = this;
            //页面初始化只让该函数执行一次，否则就会导致多次绑定点击事件出问题
            if (this.controlOnce) {
                this.controlOnce = false;
                var hosEl = document.querySelector(options.hosEl);
                var lis = hosEl.children[0].children;
                var lisLen = lis.length;
                var width = 0;
                var breakFlag = true;
                for (var i = 0; i < lisLen; i++) {
                    width += lis[i].offsetWidth;
                    //当显示的最后一个li距离屏幕距离很近时特殊处理
                    if (Math.abs(width - window.innerWidth) < 15) {
                        that.liNum = i + 1;
                        breakFlag = false;
                    }
                };
                
                for (var i = 0; i < lisLen; i++) {
                    if (breakFlag) {
                        //当当前屏幕宽度处在某两个li的offsetLeft范围之间时，就记录当前li的索引值，用于计算超出屏幕的li的个数
                        if (lis[i].offsetLeft > window.innerWidth && lis[i-1].offsetLeft <= window.innerWidth) {
                            that.liNum = i;
                        } 
                    }
                    
                };
                //判断当前移动系统安卓或者ios
                function confirmOS() {  
                    var u = navigator.userAgent;
                    if (u.indexOf('Android') > -1 || u.indexOf('Linux') > -1) {//安卓手机
                        return 1;
                    } else if (u.indexOf('iPhone') > -1) {//苹果手机
                        return 2
                    } else if (u.indexOf('Windows Phone') > -1) {//winphone手机
                        return 3
                    }
                }
                //由于在ios上ul的宽度设置后偏小，一行放不下，所以在ios上多加几个像素
                var navUlWidth = confirmOS() == 1 ? (width + 2) : (width + 4);
                //创建导航栏水平滚动实例
                hosEl.children[0].style.width = navUlWidth + 'px';
                that.navScroll = new BScroll(hosEl,{
                    scrollX: true,
                    scrollY: false,
                    freeScroll:true,
                    click: true,
                    bounce: {
                        left: false,
                        right: false
                    }
                });

                //绑定导航栏li的点击事件
                that.changeNavList(options); 
                //当点击导航栏li结束时就放开对内容滚动区域导致的导航栏滑动事件的限制
                that.navScroll.on('touchEnd',function () {  
                    //此处加上延时是关键，因为移动端的click事件比touchend事件延迟300ms，
                    // 所以当点击过li时，如果不加延迟就会先触发touchend事件后触发click事件使得clickFlag=true，
                    // 导致点击过后就无法响应内容滚动时导航栏的滑动了
                    setTimeout(function () {  
                        that.clickFlag = false;
                    },400)
                })
                //计算每次滑动应该滑动的距离（ul的最大可滑动距离除以未展示的li的个数）
                that.liDisX = -that.navScroll.maxScrollX/(lisLen - that.liNum);
                //获取导航栏每个li的offsetLeft的值为了在内容滚动时确定导航栏应该滚动的时间
                for (var i = 0; i < lisLen; i++) {
                    if (that.navLiLeft.indexOf(lis[i].offsetLeft) == -1) {
                        that.navLiLeft.push(lis[i].offsetLeft);
                    }
                };
            }
        },


        //导航栏与内容滚动实例
        betterScroll: function (options) {  
            var that = this;
            //注册垂直滚动实例及绑定内容滚动事件
            that.$nextTick(function () {
                var posTopEl = document.querySelector(options.posTopEl);
                var posBottomEl = document.querySelector(options.posBottomEl);
                var verEl = document.querySelector(options.verEl);
                if (!posTopEl) {
                    document.querySelector('.placeholder-header').style.display = 'none';
                    
                }  
                var windowHeight = window.innerHeight;
                //获取顶部固定定位元素的高度
                var fixedTopH = posTopEl ? posTopEl.offsetHeight : 0;
                //获取底部固定定位元素的高度
                var fixedBottom = posBottomEl ? posBottomEl.offsetHeight : 0;
                var fixedH = fixedTopH + fixedBottom;
                
                //获取顶部固定定位元素的初始定位值
                var fixedTopPos = posTopEl ? that.getStyle(posTopEl,'top') : '-50';
                
                verEl.style.height = windowHeight - fixedH + 'px';
                
                
                //创建垂直滚动实例
                that.menuScroll = new BScroll(verEl,{
                    scrollX: false,
                    scrollY: true,
                    freeScroll: true,
                    probeType: 3,   //派发实时scroll事件，只能设置为3
                    bounce: {
                        top: false
                    }
                });

                var coverH = document.querySelector(options.coverEl) ? document.querySelector(options.coverEl).offsetHeight : 0;
                var hosEl = document.querySelector(options.hosEl);
                
                //注册滚动事件
                that.menuScroll.on('scroll', function (pos) {  
                    var disY = Math.abs(pos.y);
                    if (pos.y <= -coverH) {
                        if (hosEl.getAttribute('scroll') == '0') {
                            //此处不使用显示与隐藏的原因是，当导航栏隐藏后之前添加的事件会失效，
                            // 但是如果每次显示时再绑定事件又会出现事件多次绑定的问题，所以使导航栏初始存在，位置在屏幕之外
                            that.showUl(options);  //内部只执行一次
                            hosEl.setAttribute('scroll', '1');
                            // hosEl.animate({'top': fixedTopH, 'opacity':'1', 'zIndex': '800'}, 10);
                            hosEl.classList.remove('hide-nav');
                            hosEl.classList.add('show-nav');
                        }
                    }else{
                        hosEl.setAttribute('scroll', '0');
                        
                        // $(options.hosEl).animate({'top': fixedTopPos, 'opacity':'0', 'zIndex': '0'}, 10);
                        hosEl.classList.remove('show-nav');
                        hosEl.classList.add('hide-nav');
                    }
                    //设置当前被激活的索引值
                    that.navList.forEach((ele, index)=>{
                        ele.key = false;
                        //判断时减5的原因是滚动时对应的值会比获取到的内容菜单的值要大一点，不符合要求
                        if (disY < (that.menuItemTop[index+1] - 5) && disY >= (that.menuItemTop[index] - 5)) {
                            that.navList[index].key = true;
                            that.navLiActive = index;
                        }else if (disY >= (that.menuItemTop[that.navList.length-1] - 5)) {
                            that.navList[that.navList.length-1].key = true;
                            that.navLiActive = that.navList.length-1;
                        }
                        
                    })

                    //当内容区域从下往上滑时，当激活索引值变化时，就让菜单栏滚动一次
                    if (that.menuScroll.movingDirectionY == 1) {
                        // 当前激活索引值的li到左侧屏幕的距离，大于屏幕宽度一半时才允许滑动
                        if (that.navLiLeft[that.navLiActive] > window.innerWidth/2) {
                            if (that.navLeftFlag) {
                                that.navLeftFlag = false;
                                if (that.navScroll.x > that.navScroll.maxScrollX && !that.clickFlag) {
                                    that.navScroll.scrollBy(-that.liDisX, 0, 200);
                                }
                            }         
                        }
                    }

                    //获取当前激活索引值的li到左侧屏幕的距离，小于屏幕宽度一半时才允许滑动
                    var pageX = that.navLiLeft[that.navLiActive] - Math.abs(that.navScroll.x);
                    //当内容区域从上往下滑时，当激活索引值变化时，就让菜单栏滚动一次
                    if (that.menuScroll.movingDirectionY == -1) {
                        if (pageX < window.innerWidth/2) {
                            if (that.navRightFlag) {
                                that.navRightFlag = false;
                                if (that.navScroll.x < 0 && !that.clickFlag) {
                                    that.navScroll.scrollBy(that.liDisX, 0, 200);
                                }
                            }
                        }
                    }
                })
                
                //获取内容菜单的所有直接子元素
                var menuItem = document.querySelector(options.contentEl).children;
                var len = menuItem.length;
                
                //获取需要被覆盖的元素的高度
                var coverH = document.querySelector(options.coverEl) ? document.querySelector(options.coverEl).offsetHeight : 0;
                //获取顶部固定定位元素的高度和被覆盖的元素高度之和
                var height = fixedTopH + coverH;
                
                for (var i = 0; i < len; i++) {
                    //记录每个内容菜单项的offsetTop值
                    that.menuItemTop.push(menuItem[i].offsetTop - height - 5);
                };
                
                //设置最后一个菜单项的多余高度，使其可以滚动到顶部
                var lastLiH = len - 1;
                var space = options.contentListSpace || 0;
                var setLastLiH = windowHeight - fixedH - document.querySelector(options.hosEl).offsetHeight - space;
                document.querySelector(options.contentEl).children[lastLiH].style.height = setLastLiH + 'px';
                
            })
        }
    },

    watch: {
        //监控被激活索引值的实时变化，重要
        navLiActive: function (newVal,oldVal) { 
            var numL = 0;
            var numR = 0;
            //判断左滑时当某个li的offsetLeft值大于屏幕宽度一半时就开始滑动
            if (this.menuScroll.movingDirectionY == 1) {
                for (var i = 0; i < this.navLiLeft.length; i++) {
                    if (this.navLiLeft[i] > window.innerWidth/2) {
                        numL = i;
                        break;
                    }
                };
                // 当某个li的offsetLeft值大于屏幕宽度一半时才允许滑动
                if (newVal >= numL ) {
                    this.navLeftFlag = true;
                }
            }

            //当右滑时进行反向判断，当索引所在li距离屏幕左侧距离小于屏幕宽度一半时就开始滑动
            if (this.menuScroll.movingDirectionY == -1) {
                for (var i = this.navLiLeft.length - 1; i > 0; i--) {
                    var pageX = this.navLiLeft[i] - Math.abs(this.navScroll.x);
                    if (pageX < window.innerWidth/2) {
                        numR = i;
                        break;
                    }
                };
                // 索引所在li距离屏幕左侧距离小于屏幕宽度一半时才允许滑动
                if (newVal <= numR) {
                    this.navRightFlag = true;
                }
            }
        }
    },

    created () {
        //实例化滚动插件
        this.betterScroll({
            hosEl: '.nav-fixed',   //水平方向导航菜单滚动元素
            verEl: '.tax-content',    //垂直方向内容滚动元素
            // posTopEl: '.user-title',  //存在的顶部固定定位元素，不存在可不传
            // posBottomEl: '.bar-tab',  //存在的底部固定定位元素，不存在可不传
            contentEl: '.menu-wrap',  //内容滚动列表的外层包裹元素
            coverEl: '.search',   //存在的需要被导航栏覆盖的元素，不存在可不传
            contentListSpace: 18  //内容列表之间的间距，随自己的设置调整
        });
        
    }
}
</script>

<style>

.content{
    background-color: #fbfafa;
    overflow-y: auto;
}

.content-block{
    margin: 0;
    padding: 0;
}

.nav{
    width: 100%;
    padding: .3rem 0 .5rem;
    line-height: 2rem;
    text-align: center;
}

.nav-item{
    display: inline-block;
    vertical-align: middle;
    line-height: 2rem;
    position: relative;
    margin: 0 .5rem;
}

.nav-item.active::after{
    content: "";
    position: absolute;
    bottom: -.15rem;
    left: 0;
    width: 100%;
    height: .15rem;
    background-color: #4e89f5;
}

.nav-item span{
    color: #4e89f5;
    font-weight: bold;
}

.nav-item img{
    width: 1rem;
    height: 1rem;
    vertical-align: middle;
}


.search{
    width: 100%;
    height: 2rem;
    padding: 0 .75rem;
    display: -webkit-flex;
    display: flex;
    justify-content: space-between;
    align-items: flex-end;
    background-color: #fff;
    position: relative;
    z-index: 500;
}

.search-icon{
    width: 1.8rem;
}

.search .iconfont{
    font-size: 1.2rem;
    position: relative;
    bottom: -.1rem;
}

.search-input{
    width: 100%;
    height: 1.4rem;
    position: relative;
}

.search-input input{
    width: 100%;
    height: 1.4rem;
    background-color: #f6f6f6;
    border-radius: .7rem;
    border: none;
    text-align: center;
    font-size: .7rem;
}

.search-input .iconfont{
    font-size: .8rem;
    color: #bcbcbd;
    position: absolute;
    left: 50%;
    top: 50%;
    margin-left: -4.8rem;
    transform: translateY(-55%);
}

.menu-box{
    width: 100%;
    padding-bottom: .5rem;
}

.menu-item{
    background-color: #fff;
    margin-bottom: .5rem;
}

.menu-item h4{
    height: 3rem;
    padding: .5rem .75rem;
    line-height: 2rem;
    font-size: .8rem;
    color: #000;
    text-align: left;
}

.menu-item h4 span{
    padding-bottom: .4rem;
    border-bottom: 2px solid #4e89f5;
}

.menu-item .item-ul li{
    width: 100%;
    height: 3.2rem;
    border-top: 1px solid #fbfafa;
    display: -webkit-flex;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.menu-item .item-ul li div{
    width: 50%;
    height: 100%;
    padding: 0 .75rem;
    line-height: 1rem;
    display: -webkit-flex;
    display: flex;
    justify-content: flex-start;
    align-items: center;
}

.menu-item .item-ul li div:first-child{
    border-right: 1px solid #fbfafa;
}

.menu-item .item-ul li span{
    padding-left: .5rem;
    font-size: .7rem;
    color: #000;
    line-height: 1rem;
}

.menu-item .item-ul li img{
    width: 2.1rem;
    height: 2.1rem;
}

.menu-item:last-child .item-ul li:last-child{
    border-bottom: 1px solid #fbfafa;
}


.nav-fixed{
    width: 100%;
    position: fixed;
    height: 2.4rem;
    line-height: 2.4rem;
    border-bottom: 1px solid #f1f1f1;
    left: 0;
    top: -50px;
    z-index: 0;
    background-color: #fff;
    opacity: 0;
}

.nav-fixed.show-nav{
    top: 0;
    opacity: 1;
    z-index: 800;
    transition: all 10;
}

.nav-fixed.hide-nav{
    top: -50px;
    opacity: 0;
    z-index: 0;
    transition: all 10;
}

.nav-ul{
    width: 300%;
    background-color: #fff;
    position: relative;
}

.nav-ul li{
    height: 2.4rem;
    float: left;
    padding: 0 .75rem;
    color: #000;
    font-size: .8rem;
    position: relative;
}

.nav-ul li.active{
    color: #4e89f5;
}

.nav-ul li.active::after{
    content: "";
    position: absolute;
    width: 100%;
    height: 2px;
    bottom: 0;
    left: 0;
    background-color: #4e89f5;
}


</style>

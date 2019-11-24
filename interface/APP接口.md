### APP接口
>   特殊请求的接口

1.  生成分享URL

    *   链接

        https://203.119.144.29/gw/mtop.ali.qrcode.genshareurl/1.1/?data=%7B%22params%22%3A%22%7B%5C%22newurl%5C%22%3A%5C%22https%3A%2F%2Fm.1688.com%2Foffer%2F601865198188.html%3Frpg-cnt%3Dshare.offerDetail%26share_business_id%3D_offerdetail%5C%22%7D%22%7D
---
2.  生成淘口令
    
    *   链接

        https://203.119.144.29/gw/mtop.alibaba.china.activity.sharetoken.create/1.1/?data=%7B%22rightBtnText%22%3A%22%E7%AB%8B%E5%8D%B3%E6%9F%A5%E7%9C%8B%22%2C%22iconLink%22%3A%22https%3A%2F%2Fcbu01.alicdn.com%2Fimg%2Fibank%2F2019%2F812%2F678%2F11899876218_484149936.310x310.jpg%22%2C%22title%22%3A%22%E5%A5%BD%E5%8F%8B%E5%88%86%E4%BA%AB%E7%9A%84%E5%95%86%E5%93%81%22%2C%22source%22%3A%22_offerdetail%22%2C%22leftBtnText%22%3A%22%E5%8F%96%E6%B6%88%22%2C%22rightBtnLink%22%3A%22https%3A%2F%2Fqr.1688.com%2Fshare.html%3Fsecret%3DDlV9b37x%22%2C%22startTime%22%3A%220%22%2C%22content%22%3A%22%E7%9F%B3%E5%A2%A8%E7%83%AF%E5%86%85%E8%A3%A4%20%E5%A5%B3%E4%B8%AD%E8%85%B0%E7%BA%AF%E8%89%B2%E5%A5%B3%E5%A3%AB%E5%86%85%E8%A3%A4%E6%97%A5%E7%B3%BB%E5%98%B4%E5%94%87%E5%8D%B0%E8%8A%B1%E5%B0%91%E5%A5%B3%E4%B8%89%E8%A7%92%E8%A3%A4%E6%96%B0%E6%AC%BE%20%E6%8A%97%E8%8F%8C%22%2C%22bizType%22%3A%22SHORT%22%7D
---
11. 获取详情

    -   URL

        https://203.119.144.29/gw/mtop.1688.wosc.cbu.offerdetailservice.queryofferdetail/1.0/?data=%7B%22responseClass%22%3A%22%5C%22com.alibaba.wireless.detail.netdata.offerdatanet.OfferDetailDataResponse%5C%22%22%2C%22RESPONSE_DATA_KEY%22%3A%22%22%2C%22MOCK_DATA%22%3A%22false%22%2C%22offerId%22%3A%22601865198188%22%7D
    ---
12. 一淘获取热门搜索词

    -   URL

        https://acs.m.taobao.com/gw/mtop.etao.fe.hotwords/2.0/?data=%7B%22lastData%22%3A%22%22%2C%22count%22%3A%2210%22%7D
    ---
13. 一淘搜索商品

    -   URL

        https://acs.m.taobao.com/gw/mtop.etao.fe.search/4.0/?data=%7B%22saleType%22%3A%22%22%2C%22src%22%3A%22android%22%2C%22pageSize%22%3A%2220%22%2C%22q%22%3A%22%E7%94%B7%E4%B8%BB%E6%92%AD%22%2C%22searchType%22%3A%220%22%2C%22lastData%22%3A%22%22%2C%22sort%22%3A%22default%22%2C%22page%22%3A%221%22%2C%22benifitType%22%3A%220%22%7D
    
    -   说明

        benifitType参数代表着搜索类型 2 优惠券 1 高返利 0 无
    ---
14. 一淘大额券搜索
    
    -   URL

        https://acs.m.taobao.com/gw/mtop.alimama.union.xt.en.api.entry/1.0/?data=%7B%22pSize%22%3A%2220%22%2C%22refpid%22%3A%22%22%2C%22count%22%3A%22200%22%2C%22appPvid%22%3A%221002.12538795_1574434542686_6019186191171553_%22%2C%22spm%22%3A%221002.12538795.18316373%22%2C%22ctm%22%3A%22spm-url%3A1002.9499542.1998742058.2%22%2C%22floorId%22%3A%2213671%22%2C%22pNum%22%3A%220%22%7D
---
15. 一淘 获取我的订单

    -   URL

        https://trade-acs.m.taobao.com/gw/mtop.trade.querybag/5.0/?data=%7B%22isPage%22%3A%22true%22%2C%22exParams%22%3A%22%7B%5C%22globalSell%5C%22%3A%5C%221%5C%22%2C%5C%22mergeCombo%5C%22%3A%5C%22true%5C%22%2C%5C%22version%5C%22%3A%5C%221.1.1%5C%22%7D%22%2C%22netType%22%3A%221%22%2C%22cartFrom%22%3A%22default_client%22%2C%22extStatus%22%3A%220%22%7D
    ---
16. 手淘  偷淘金币

    -   URL

        https://h5api.m.taobao.com/h5/mtop.coingame.farm.behavior.steal/1.0/?jsv=2.5.0&appKey=12574478&t=1574437381903&sign=c04e1e35e1682fc0e1db89e7ce3785f6&v=1.0&api=mtop.coingame.farm.behavior.steal&type=jsonp&dataType=jsonp&callback=mtopjsonp6&data=%7B%22bizCode%22%3A%22taoCoin%22%2C%22subBizCode%22%3A%22farm%22%2C%22friendId%22%3A%222290481412%22%2C%22vegeId%22%3A%2231235248355%22%7D
    
    -   来源：

        https://market.m.taobao.com/app/tmall-wireless/tjb-2018/index/index.html?disableNav=YES#/tjb
---
17. 手淘 商品评论

    -   URL

        https://guide-acs.m.taobao.com/gw/mtop.taobao.rate.detaillist.get/5.0/?data=%7B%22rateSrc%22%3A%22shoutao_rate_list%22%2C%22promoteFeedId%22%3A%221065640633649%22%2C%22pageSize%22%3A%2210%22%2C%22invokeSource%22%3A%223%22%2C%22feedId%22%3A%221065640633649%22%2C%22hasPic%22%3A%221%22%2C%22pageNo%22%3A%221%22%2C%22foldFlag%22%3A%220%22%2C%22rateType%22%3A%22%22%2C%22auctionNumId%22%3A%22606835501951%22%7D
    ---
18. 手淘 获取直播详情

    -   URL

        https://guide-acs.m.taobao.com/gw/mtop.mediaplatform.live.livedetail/4.0/?data=%7B%22extendJson%22%3A%22%7B%5C%22guardAnchorSwitch%5C%22%3Atrue%2C%5C%22version%5C%22%3A%5C%22201903%5C%22%7D%22%2C%22ignoreH265%22%3A%22false%22%2C%22liveId%22%3A%22222640107253%22%7D
---
19. 手淘 获取店铺信息

    -   URL

        https://guide-acs.m.taobao.com/gw/mtop.taobao.wireless.shop.fetch/2.0/?data=%7B%22originUrl%22%3A%22%22%2C%22shopId%22%3A%2236529258%22%2C%22sellerId%22%3A%2227796690%22%2C%22features%22%3A%22%7B%7D%22%2C%22shopNavi%22%3A%22%22%7D
---
20. 手淘 获取店铺微淘群

    -   URL

        https://h5api.m.taobao.com/h5/mtop.taobao.chatting.group.middlepage/1.0/?jsv=2.5.1&appKey=12574478&t=1574439809172&sign=2d67e22883e54c541f3e75295d506f6f&api=mtop.taobao.chatting.group.middlepage&v=1.0&type=jsonp&dataType=jsonp&timeout=10000&callback=mtopjsonp1&data=%7B%22groupId%22%3A%220_V_27796690_1560476556347%22%7D
    -   来源

        https://market.m.taobao.com/app/tb-source-app/shopindex/pages/index?alisite=true&wh_weex=true&videoDowngrade=true&hideHeader=true&hiddenTab=false&shopId=36529258&pageId=84044019&pathInfo=shop/index&userId=27796690&isCompatible=true
---
21. 手淘 进入微淘群

    -   URL

        https://h5api.m.taobao.com/h5/mtop.taobao.social.follow.weitao.add/3.1/?jsv=2.5.1&appKey=12574478&t=1574439983732&sign=79da57603c8e07fb87c04a7fe73d0fc2&api=mtop.taobao.social.follow.weitao.add&v=3.1&ecode=1&type=jsonp&dataType=jsonp&timeout=10000&callback=mtopjsonp2&data=%7B%22accountType%22%3A2%2C%22pubAccountId%22%3A%2227796690%22%2C%22originBiz%22%3A%22qunliao%22%2C%22originFlag%22%3A%22unknown%22%7D
    ---
    
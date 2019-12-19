<template>
    <div style="float:left;margin-left:50px">
        <el-row>
            <el-row style="margin-left: 2px">
                <h2 style="width: 180px;">豆瓣电影排行榜</h2>
                <p style="color:green;width: 150px">豆瓣新片榜· · · · · · </p>
            </el-row>
            <hr style="border: 0.5px dashed #cfc7dd;margin-left: 1px;width: 900px;">
            <el-row v-for="List in moodList" type="flex" justify="left" :gutter="20"
                    style="margin-top: 20px;margin-left: 5px">
                <el-col :span="4">
                    <img v-bind:src="List[0].imgUrl"style="width: 130px;height:200px;" />
                </el-col>
                <el-col :span="11" style="text-align: left;padding-left: 1px;margin-left: 50px;margin-top: 10px">
                    <a href="#" style="text-decoration: none"><div class="ab">{{List[0].name}}</div></a>
                    <p style="margin-top: 15px;color:#666666">
                        {{List[0].actor}}
                    </p>
                    <el-rate
                            style="margin-top:50px"
                            disabled
                            text-color="#f90"
                            v-model="List[0].score">
                    </el-rate>
                    <div style="margin-top: -21px;margin-left: 130px"><a style="color: #b88b1f">4.4</a>  &nbsp;(123358人评价)</div>
                </el-col>
            </el-row>
            <hr style="border: 0.5px dashed #cfc7dd;margin-left: 1px;width: 900px;">
            <el-row v-for="List in moodList" type="flex" justify="left" :gutter="20"
                    style="margin-top: 20px;margin-left:5px">
                <el-col :span="4">
                    <img v-bind:src="List[1].imgUrl"style="width: 130px;height:200px;" />
                </el-col>
                <el-col :span="11" style="text-align: left;padding-left: 1px;margin-left: 50px;margin-top: 10px">
                    <a href="#" style="text-decoration: none"><div class="ab">{{List[1].name}}</div></a>
                    <p style="margin-top: 15px;color:#666666">
                        {{List[1].actor}}
                    </p>
                    <el-rate
                            style="margin-top:50px"
                            disabled
                            text-color="#ff9900"
                            v-model="List[1].score">
                    </el-rate>
                    <div style="margin-top: -21px;margin-left: 130px"><a style="color: #b88b1f">4.1</a>  &nbsp;(256214人评价)</div>
                </el-col>
            </el-row>
            <hr style="border: 0.5px dashed #cfc7dd;margin-left: 1px;width: 900px;">
            <el-row v-for="List in moodList" type="flex" justify="left" :gutter="20"
                    style="margin-top: 20px;margin-left: 5px">
                <el-col :span="4">
                    <img v-bind:src="List[2].imgUrl"style="width: 130px;height:200px;" />
                </el-col>
                <el-col :span="11" style="text-align: left;padding-left: 1px;margin-left: 50px;margin-top: 10px">
                    <a href="#" style="text-decoration: none"><div class="ab">{{List[2].name}}</div></a>
                    <p style="margin-top: 15px;color:#666666">
                        {{List[2].actor}}
                    </p>
                    <el-rate
                            style="margin-top:50px"
                            disabled
                            text-color="#f90"
                            v-model="List[2].score">
                    </el-rate>
                    <div style="margin-top: -21px;margin-left: 130px"><a style="color: #b88b1f">3.8</a>  &nbsp;(698547人评价)</div>
                </el-col>
            </el-row>
            <hr style="border: 0.5px dashed #cfc7dd;margin-left: 1px;width: 900px;">
            <el-row v-for="List in moodList" type="flex" justify="left" :gutter="20"
                    style="margin-top: 20px;margin-left: 5px">
                <el-col :span="4">
                    <img v-bind:src="List[3].imgUrl"style="width: 130px;height:200px;" />
                </el-col>
                <el-col :span="11" style="text-align: left;padding-left: 1px;margin-left: 50px;margin-top: 10px">
                    <a href="#" style="text-decoration: none"><div class="ab">{{List[3].name}}</div></a>
                    <p style="margin-top: 15px;color:#666666">
                        {{List[3].actor}}
                    </p>
                    <el-rate
                            style="margin-top:50px"
                            disabled
                            text-color="#f90"
                            v-model="List[3].score">
                    </el-rate>
                    <div style="margin-top: -21px;margin-left: 130px"><a style="color: #b88b1f">3.7</a>  &nbsp;(365241人评价)</div>
                </el-col>
            </el-row>
            <hr style="border: 0.5px dashed #cfc7dd;margin-left: 1px;width: 900px;">
            <el-row v-for="List in moodList" type="flex" justify="left" :gutter="20"
                    style="margin-top: 20px;margin-left: 5px">
                <el-col :span="4">
                    <img v-bind:src="List[4].imgUrl"style="width: 130px;height:200px;" />
                </el-col>
                <el-col :span="11" style="text-align: left;padding-left: 1px;margin-left: 50px;margin-top: 10px">
                    <a href="#" style="text-decoration: none;"><div class="ab">{{List[4].name}}</div></a>
                    <p style="margin-top: 15px;color:#666666">
                        {{List[4].actor}}
                    </p>
                    <el-rate
                            style="margin-top:50px"
                            disabled
                            text-color="#ff9900"
                            v-model="List[4].score">
                    </el-rate>
                    <div style="margin-top: -21px;margin-left: 130px"><a style="color: #b88b1f">3.6</a>  &nbsp;(756214人评价)</div>
                </el-col>
            </el-row>
            <hr style="border: 0.5px dashed #cfc7dd;margin-left: 1px;width: 900px;">
            <el-row v-for="List in moodList" type="flex" justify="left" :gutter="20"
                    style="margin-top: 20px;margin-left: 5px">
                <el-col :span="4">
                    <img v-bind:src="List[5].imgUrl"style="width: 130px;height:200px;" />
                </el-col>
                <el-col :span="11" style="text-align: left;padding-left: 1px;margin-left: 50px;margin-top: 10px">
                    <a href="#" style="text-decoration: none"><div class="ab">{{List[5].name}}</div></a>
                    <p style="margin-top: 15px;color:#666666">
                        {{List[5].actor}}
                    </p>
                    <el-rate
                            style="margin-top:50px"
                            disabled
                            text-color="#f90"
                            v-model="List[5].score">
                    </el-rate>
                    <div style="margin-top: -21px;margin-left: 130px"><a style="color: #b88b1f">2.1</a>  &nbsp;(222549人评价)</div>
                </el-col>
            </el-row>
            <hr style="border: 0.5px dashed #cfc7dd;margin-left: 1px;width: 900px;">
        </el-row>
    </div>
</template>
<script>
    export default{
        data:function(){
            return{
                moodList:[
                    [
                        {
                            name:'爱尔兰杀手(港) / 听说你刷房子了',
                            score:4.4,
                            imgUrl:require('../assets/6.jpg'),
                            actor:"2019-09-27(纽约电影节) / 2019-11-01(美国点映) / 2019-11-27(美国网络) / 罗伯特·德尼罗 / 阿尔·帕西诺 / 乔·佩西 / 安娜·帕奎因 / 杰西·普莱蒙 / 哈威·凯特尔 / 斯蒂芬·格拉汉姆 / 鲍比·坎纳瓦尔 / 杰克·休斯顿 / 阿莱卡萨·帕拉迪诺 / 凯瑟琳·纳杜奇..."
                        },
                        {
                            name:'小丑起源电影：罗密欧/Romeo',
                            score:4.1,
                            imgUrl:require('../assets/1.jpg'),
                            actor:"2019-08-31(威尼斯电影节) / 2019-10-04(美国) / 杰昆·菲尼克斯 / 罗伯特·德尼罗 / 马克·马龙 / 莎姬·贝兹 / 谢伊·惠格姆 / 弗兰西丝·康罗伊 / 布莱恩·考伦 / 布莱恩·泰里·亨利 / 布莱特·卡伦 / 道格拉斯·霍奇斯 / 格伦·弗莱施勒 / 比尔·坎普..."
                        },
                        {
                            name:'双子杀手/2019-11-7(香港)',
                            score:3.8,
                            imgUrl:require('../assets/10.jpg'),
                            actor:"2019-10-23(中国) / 2019-11-07(中国香港) / 郑有美 / 孔侑 / 金美京 / 孔敏晶 / 朴成妍 / 李凤莲 / 金圣喆 / 李乌 / 李海云 / 孙成灿 / 金正英 / 李娜云 / 禹志贤 / 韩国 / 金度英 / 118分钟 / 82年生的金智英 / 剧情 / 刘英雅 Yeong-ah Yoo / 赵南珠 Nam-joo..."
                        },
                        {
                            name:' 好莱坞往事/Romeo(戛纳电影节) ',
                            score:3.7,
                            imgUrl:require('../assets/2.jpg'),
                            actor:"2019-05-21(戛纳电影节) / 2019-07-26(美国) / 2019(中国大陆) / 莱昂纳多·迪卡普里奥 / 布拉德·皮特 / 玛格特·罗比 / 埃米尔·赫斯基 / 玛格丽特·库里 / 蒂莫西·奥利芬特 / 茱莉亚·巴特斯 / 奥斯汀·巴特勒 / 达科塔·范宁 / 布鲁斯·邓恩 /..."
                        },
                        {
                            name:'我在你床上and床下/Romeo/鬼子',
                            score:3.6,
                            imgUrl:require('../assets/4.jpg'),
                            actor:"2019-08-31(威尼斯电影节) / 2019-10-04(美国) / 杰昆·菲尼克斯 / 罗伯特·德尼罗 / 马克·马龙 / 莎姬·贝兹 / 谢伊·惠格姆 / 弗兰西丝·康罗伊 / 布莱恩·考伦 / 布莱恩·泰里·亨利 / 布莱特·卡伦 / 道格拉斯·霍奇斯 / 格伦·弗莱施勒 / 比尔·坎普..."
                        },
                        {
                            name:'非凡夏日',
                            score:2.1,
                            imgUrl:require('../assets/3.jpg'),
                            actor:"2019-08-29(威尼斯电影节) / 2019-12-06(美国) / 斯嘉丽·约翰逊 / 亚当·德赖弗 / 梅里特·韦弗 / 劳拉·邓恩 / 雷·利奥塔 / 朱丽·哈基提 / 马克·奥布莱恩 / 华莱士·肖恩 / 阿伦·阿尔达 / 凯尔·柏海莫 / 米奇·萨姆纳 / 艾奇·罗伯逊 / 马修·马希尔..."
                        },
                    ]
                ]
            }
        }

    }
</script>
<style>
    .ab{font-family:"幼圆";color:#37a}
    .ab:hover{background-color: rgb(152, 208, 233);width:260px  }
</style>
<template>
    <div class="youyu-content" id="imgLazy">
        <ul class="lazy-img-wrap">
            <li v-for="(list, index) in imgList" :key="index">
                <img v-lazyload.imgLazy="list" class="lazy-img" alt="">
            </li>
        </ul>
    </div>
</template>

<script>
'use strict'

export default {
    data: () => ({
        imgList: [
            "https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1491153876796&di=bc888f2b6675f77d0d631d1579a40da2&imgtype=0&src=http%3A%2F%2Fimgnews.gmw.cn%2Fattachement%2Fjpg%2Fsite2%2F20160512%2F4489700852197339238.jpg",
            "https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1491153875644&di=18ee80e3f6d2604f02adaebb85dcc28e&imgtype=0&src=http%3A%2F%2Fimg3.duitang.com%2Fuploads%2Fitem%2F201511%2F09%2F20151109100605_jfmaK.jpeg",
            "https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1491153875640&di=267e5a70bb0b3d0b0e845b786406704f&imgtype=0&src=http%3A%2F%2Fwww.t-cha.com%2FtutcL3R1dGNpbWcwMi50YW9iYW9jZG4uY29tL2Jhby91cGxvYWRlZC9pMi9UQjF1UmZXRlZYWFhYY1dYRlhYWFhYWFhYWFhfISEwLWl0ZW1fcGljLmpwZw%3D%3D.jpg",
            "https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1491153875639&di=d76c80867ab3271473c1a836e96979ff&imgtype=0&src=http%3A%2F%2Fimg3.duitang.com%2Fuploads%2Fitem%2F201511%2F09%2F20151109100823_JGKTw.jpeg",
            "https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1491153875639&di=5ce79d4225315c7c4a27f93b063d1aff&imgtype=0&src=http%3A%2F%2Fimg3.duitang.com%2Fuploads%2Fitem%2F201511%2F09%2F20151109104354_TLyKu.jpeg"
        ]
    }),
    methods: {
        addList() {
            var arr = [
                "https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1491153876796&di=bc888f2b6675f77d0d631d1579a40da2&imgtype=0&src=http%3A%2F%2Fimgnews.gmw.cn%2Fattachement%2Fjpg%2Fsite2%2F20160512%2F4489700852197339238.jpg",
                "https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1491153875644&di=18ee80e3f6d2604f02adaebb85dcc28e&imgtype=0&src=http%3A%2F%2Fimg3.duitang.com%2Fuploads%2Fitem%2F201511%2F09%2F20151109100605_jfmaK.jpeg",
                "https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1491153875640&di=267e5a70bb0b3d0b0e845b786406704f&imgtype=0&src=http%3A%2F%2Fwww.t-cha.com%2FtutcL3R1dGNpbWcwMi50YW9iYW9jZG4uY29tL2Jhby91cGxvYWRlZC9pMi9UQjF1UmZXRlZYWFhYY1dYRlhYWFhYWFhYWFhfISEwLWl0ZW1fcGljLmpwZw%3D%3D.jpg",
                "https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1491153875639&di=d76c80867ab3271473c1a836e96979ff&imgtype=0&src=http%3A%2F%2Fimg3.duitang.com%2Fuploads%2Fitem%2F201511%2F09%2F20151109100823_JGKTw.jpeg",
                "https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1491153875639&di=5ce79d4225315c7c4a27f93b063d1aff&imgtype=0&src=http%3A%2F%2Fimg3.duitang.com%2Fuploads%2Fitem%2F201511%2F09%2F20151109104354_TLyKu.jpeg"
            ]
            this.imgList = this.imgList.concat(arr);
            this.ImgLazyLoad.resize();
        }
    }
}

</script>


<style>
.lazy-img-wrap{
    width: 100%;
}
.llazy-img-wrap li{
    width: 100%;
}
.lazy-img-wrap li img{
    width: 100%;
}
</style>

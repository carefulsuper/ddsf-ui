<template>
    <div class="m-card" :style="width? {width: width + 'px'}: {}">
        <div class="m-card-img" :style="imgHeight? {height: imgHeight + 'px'} : {}">
            <img :src="imgSrc" alt="image"/>
        </div>
        <div v-if="summary" class="m-card-summary">
            {{summary}}
        </div>
        <div v-else>
            <slot></slot>
        </div>
        <slot name="footer"></slot>
    </div>
</template>

<script>
export default {
    name: 'm-card',
    props: {
        width: { // 卡片宽度
            type: Number,
            default: 0
        },
        imgSrc:{ // 卡片资源链接
            type: String,
            default:''
        },
        imgHeight: { // 卡片的高度
            type: Number,
            default: 0
        },
        summary:{ // 卡片概要
            type: String,
            default: ''
        }
    }
}
</script>
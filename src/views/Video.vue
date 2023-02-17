
<template >
    <div>
    <vue3VideoPlay
      v-bind="options"
      poster="https://cdn.jsdelivr.net/gh/xdlumia/files/video-play/ironMan.jpg"
    />
    
  </div>
</template>
<script lang="ts" setup>
import { reactive } from "vue";
const options = reactive({
  width: "500px", //播放器高度
  height: "260px", //播放器高度
  color: "#409eff", //主题色
  currentTime: 60,
//   speed: false, //关闭进度条拖动
  speed: true, //关闭进度条拖动
  title: "", //视频名称
//   src: "https://cdn.jsdelivr.net/gh/xdlumia/files/video-play/IronMan.mp4", //视频源
  src: "http://127.0.0.1:9200/player/video",
});
</script>
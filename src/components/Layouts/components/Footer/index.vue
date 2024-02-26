<template>
  <div class="footer">
    <a-row>
      <a-col v-for="list in lists" :key="list" span="6">
        <ul :style="{ listStyle: 'none' }">
          <h2 :style="{ color: '#fff' }">{{ list.title }}</h2>
          <li v-for="content in list.content" :key="content">{{ content }}</li>
        </ul>
      </a-col>
    </a-row>

    <div :style="{ textAlign: 'center' }">
      © 慕课网（imooc.com）版权所有 | 津ICP备20000929号-2 购买课程 作业和打卡
      开源仓库 帮助
    </div>
  </div>
</template>

<script setup lang="ts">

const lists = [
  {
    title: '购买课程',
    content: ['购买课程', '作业和打卡', '开源仓库', '帮助'],
  },
  {
    title: '作业和打卡',
    content: ['购买课程', '作业和打卡', '开源仓库', '帮助'],
  },
  {
    title: '开源仓库',
    content: ['购买课程', '作业和打卡', '开源仓库', '帮助'],
  },
  {
    title: '帮助',
    content: ['购买课程', '作业和打卡', '开源仓库', '帮助'],
  },
];



</script>
<style>
@import './index.scss';
</style>
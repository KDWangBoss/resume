<template>
  <div class="menu">
    <div v-for="(menuProp, menuPropIndex) in menuProps" 
         :key="menuPropIndex"
         class="bg-[#e8e8e8] text-center w-28px text-12px ml-2px"
         @click="onMenuPropClick(menuPropIndex)">
          {{ menuProp.name }}
        </div>
  </div>
</template>

<script>
export default {
  name: 'Menu',
  data() {
    return {
      menuProps: [
        { name: '个人简历说明' },
        { name: '基本信息' },
        { name: '个人技能' },
        { name: '工作经历' },
        { name: '项目经历' },
        { name: '教育背景' },
      ],
    };
  },
  methods: {
    onMenuPropClick() {

    }
  },
  mounted() {
    // Code to run when the component is mounted goes here
  },
};
</script>

<style scoped>
/* Your component styles go here */
</style>
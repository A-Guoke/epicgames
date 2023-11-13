<!-- 原生可拖拽表格 -->
<template>
  <div>
    <div class="title">鼠标放到ID列和行上试试 可以拖拽行和列</div>
    <table class="tb">
      <thead>
        <draggable
          v-model="state.headers"
          animation="200"
          tag="tr"
          :item-key="(key: any) => key"
        >
          <template #item="{ element: header }">
            <th class="move">
              {{ header }}
            </th>
          </template>
        </draggable>
      </thead>
      <draggable
        :list="state.list"
        handle=".move"
        animation="300"
        @start="onStart"
        @end="onEnd"
        tag="tbody"
        item-key="name"
      >
        <template #item="{ element }">
          <tr>
            <td
              class="move"
              v-for="(header) in state.headers"
              :key="header"
            >
              {{ element[header] }}
            </td>
          </tr>
        </template>
      </draggable>
    </table>
  </div>
</template>
<script lang="ts" setup>
import {  reactive } from "vue";
import draggable from "vuedraggable";
/*
draggable 对CSS样式没有什么要求万物皆可拖拽
:list="state.list"         //需要绑定的数组 
animation="300"            //动画效果
@start="onStart"           //拖拽开始的事件
@end="onEnd"               //拖拽结束的事件
*/
const state = reactive({
  //列的名称
  headers: ["id", "name", "intro"],
  //需要拖拽的数据，拖拽后数据的顺序也会变化
  list: [
    { name: "www.itxst.com", id: 0, intro: "慢吞吞的蜗牛" },
    { name: "www.baidu.com", id: 1, intro: "中文搜索引擎" },
    { name: "www.google.com", id: 3, intro: "安卓操作系统" },
  ],
});

//拖拽开始的事件
const onStart = () => {
  console.log("开始拖拽");
};

//拖拽结束的事件
const onEnd = () => {
  console.log("结束拖拽");
};
</script>
<style scoped>
.title {
  padding: 3px;
  font-size: 13px;
}
.itxst {
  width: 600px;
}

.move {
  cursor: move;
}

table.tb {
  color: #333;
  border: solid 1px #999;
  font-size: 13px;
  border-collapse: collapse;
  min-width: 500px;
  user-select: none;
}
table.tb th {
  background: rgb(168 173 217);
  border-width: 1px;
  padding: 8px;
  border-style: solid;
  border-color: #999;
  text-align: left;
}
table.tb th:nth-of-type(1) {
  text-align: center;
}
table.tb td {
  background: #d6c8c8;
  border-width: 1px;
  padding: 8px;
  border-style: solid;
  border-color: #999;
}
table.tb td:nth-of-type(1) {
  text-align: center;
}
</style>
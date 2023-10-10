<template>

  <!-- 表格 -->
  <el-table
      :data="state.UserAchieve"
      style="width: 100%"
      :key="state.dictTableKey"
      border
      :header-cell-style="{backgroundColor:'#E7F8FF',fontWeight: '500',color:'#000000'}"
  >
    <el-table-column type="index" label="序号" width="50" align="center" />
    <el-table-column prop="name" label="名称" width="150" align="center" >
      <template #default="scope">
        <el-input v-model="scope.row.name" placeholder="请填写名称" />
      </template>
    </el-table-column>
    <el-table-column prop="code" label="资格证书编号" width="150" align="center" >
      <template #default="scope">
        <el-input v-model="scope.row.code" placeholder="请填写证书编号" />
      </template>
    </el-table-column>
    <el-table-column prop="adName" label="资格评定单位名称" align="center" >
      <template #default="scope">
        <el-input v-model="scope.row.adName" placeholder="请填写评定单位" />
      </template>
    </el-table-column>
    <el-table-column label="操作" width="100" align="center">
      <template #default="scope">
        <el-button :icon="Delete" type="danger"
                   @click="deleteCgBtn(scope.row)"
        >
          删除
        </el-button>
      </template>
    </el-table-column>
  </el-table>
</template>

<script setup lang="ts">
import Sortable from 'sortablejs';
import {reactive, onMounted, watch, nextTick} from "vue";
const state = reactive({
  UserAchieve: [
      {
        index: 0,
        name: "第一",
        code: 1,
        adName: "aa"
      },
    {
      index: 1,
      name: "第二",
      code: 2,
      adName: "aa"
    },
    {
      index: 2,
      name: "第三",
      code: 3,
      adName: "aa"
    }
  ],
  dictTableKey: null
})


onMounted(() => {
  nextTick(() => {
    dragSort();
  });
})


//行拖拽
const dragSort = () => {
  let that = this;
  // 首先获取需要拖拽的dom节点
  const el1 = document.querySelectorAll('.el-table__body-wrapper')[0].querySelectorAll('table > tbody')[0];
  Sortable.create(el1, {
    disabled: false, // 是否开启拖拽
    ghostClass: 'sortable-ghost', //拖拽样式
    animation: 150, // 拖拽延时，效果更好看
    group: { // 是否开启跨表拖拽
      pull: false,
      put: false
    },
    onEnd: (evt) => { //进行数据的处理，拖拽实际并不会改变绑定数据的顺序
      const { newIndex, oldIndex } = evt
      console.log(oldIndex,newIndex)
      console.log("old",state.UserAchieve[oldIndex])
      state.UserAchieve[oldIndex].index = newIndex
      console.log("new",state.UserAchieve[newIndex])
      state.UserAchieve[newIndex].index = oldIndex
      const currRow = state.UserAchieve?.splice(oldIndex, 1)[0]
      state.UserAchieve?.splice(newIndex, 0, currRow)
      sortIndex()
    }
  });
}

const sortIndex = () => {
  const array = []
  state.UserAchieve.forEach((e, i) => {
    let obj = {
      currency_id: e.currency_id,
      index: i + 1
    }
    array.push(obj)
    state.dictTableKey++;
  })
}

watch(
    () => state.dictTableKey,
    () => {
      nextTick(() => {
        dragSort();
      });
    }
);
</script>
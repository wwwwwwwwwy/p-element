<template>
  <div>
    <p>{{checkList.join(',')}}</p>
    <el-checkbox-group v-model="checkList">
      <el-checkbox label="复选框 A"></el-checkbox>
      <el-checkbox label="复选框 B"></el-checkbox>
      <el-checkbox label="复选框 C"></el-checkbox>
      <el-checkbox label="禁用" disabled></el-checkbox>
      <el-checkbox label="选中且禁用" disabled></el-checkbox>
    </el-checkbox-group>
    <p>{{checkboxGroup.join(',')}}</p>
    <el-checkbox-group v-model="checkboxGroup" size="small">
      <el-checkbox-button
        v-for="city in cities"
        :label="city"
        :disabled="city === '北京'"
        :key="city"
      >{{city}}</el-checkbox-button>
    </el-checkbox-group>
    <p>{{radio}}</p>
    <el-radio-group v-model="radio">
      <el-radio :label="3">备选项3</el-radio>
      <el-radio :label="6">备选项6</el-radio>
      <el-radio :label="9">备选项9</el-radio>
    </el-radio-group>
    <p>{{radio3}}</p>
    <el-radio-group v-model="radio3" size="small">
      <el-radio-button label="上海"></el-radio-button>
      <el-radio-button label="北京" disabled></el-radio-button>
      <el-radio-button label="广州"></el-radio-button>
      <el-radio-button label="深圳"></el-radio-button>
    </el-radio-group>
    <p>开关按钮</p>
    <el-switch v-model="switchs"></el-switch>
  </div>
</template>
<script>
export default {
  data() {
    return {
      checkList: ["选中且禁用", "复选框 A"],
      cities: ["上海", "北京", "广州", "深圳"],
      checkboxGroup: ["上海"],
      radio: 3,
      radio3: "上海",
      switchs: "是"
    };
  }
};
</script>


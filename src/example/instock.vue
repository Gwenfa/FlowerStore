<template>
<div id="table_box">
<div id="box_header">
<ul class="ul_left">
  <li>价格方式：<span>库存成本价</span></li>
</ul>
<ul class="ul_right">
   <li>
   <el-checkbox-group v-model="checkList">
    <el-checkbox label="显示停用仓库"></el-checkbox>
    <el-checkbox label="显示停用商品"></el-checkbox>
  </el-checkbox-group>
  </li>
  <li>
    <span>过滤
     <el-select v-model="value" placeholder="请选择">
       <el-option v-for="item in options" :key="item.value" :label="item.label" :value="item.value"> </el-option>
    </el-select>
    </span>
  </li>
</ul>
</div>
<div id="show_message">
  <el-table :data="tableData3" border style="width: 100%">
    <el-table-column prop="id" label="序号" width="40"></el-table-column>

    <el-table-column label="商品信息" style="text-align:center;color:red;">
      <el-table-column  prop="No" label="产品编号"  width="95"></el-table-column>
      <el-table-column prop="name"label="商品名称" width="179"></el-table-column>
      <el-table-columnprop="size" label="规格" width="95"></el-table-column>
      <el-table-column prop="version" label="型号" width="95"></el-table-column>
      <el-table-column prop="manu" label="产地" width="95"></el-table-column>
      <el-table-column prop="danwei" label="单位" width="95"></el-table-column>
    </el-table-column>

    <el-table-column label="总仓库">
      <el-table-column prop="quantity" label="数量" width="95"></el-table-column>
      <el-table-column prop="money" label="金额"  width="95"></el-table-column>
    </el-table-column>

    <el-table-column label="库房-北京站">
      <el-table-column prop="quantity2" label="数量" width="95"></el-table-column>
      <el-table-column prop="money2" label="金额" width="95"></el-table-column>
    </el-table-column>

    <el-table-column label="库房-北京站">
      <el-table-column prop="quantity3" label="数量" width="95"></el-table-column>
      <el-table-column prop="money3" label="金额" width="95"></el-table-column>
    </el-table-column>

  </el-table>
  </div>
 </div> 
</template>

<script>
  export default {
    data() {
      return {
        checkList: [],
        tableData3: [{
          id: 1,
          No: 'a710032',
          name: 'a五位荧光开光',
          size: '20*11',
          version: 'w12265d',
          manu:'中国',
          danwei:'个',
          quantity:120,
          money:9600,
          quantity:0,
          money:0,
          quantity:0,
          money:0
        }],
        options: [{
          value: '选项1',
          label: '显示全部'
        }, {
          value: '选项2',
          label: '不显示各仓库数量和金额都为0'
        }
        ]
      }
    }
  }
</script>
<style>
#table_box{
    padding: 20px 24px;
}
#show_message{
    border: 1px solid #ddd;
}
li{
  list-style: none;

}
.ul_left{
    display: inline-block;
    /*padding-bottom: 10px;*/
}
.ul_right{
  float: right;
   /*padding-bottom: 10px;*/
}
.ul_right li{
    display: inline-block;
  }

</style>
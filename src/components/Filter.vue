<template>
  <div class="custom-page">
    <h2>过滤器</h2>
    <table class="table table-bordered table-striped">
      <thead>
        <tr>
          <th class="text-center">name</th>
          <th class="text-center">初始值</th>
          <th class="text-center">保留小数点位数</th>
          <th class="text-center">小计</th>
          <th class="text-center">分类</th>
        </tr>
      </thead>
      <tbody>
<!--        <tr v-for="product in products | filterBy '苹果' in 'name'">
 -->        <tr v-for="product in products">
          <td>{{product.name}}</td>
          <td>{{product}}</td>
          <td>{{product.price | fixed | currency}}</td>
          <td>{{product.price | sum(product.price, product.num)}}</td> 
          <!-- 这里完全可以不用过滤器完成运算 -->
          <td>{{product.category | kind(product.category)}}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>


export default {

  name: 'Filter',
  data () {
    return {
      testData: 46533,
      products: [
        {name: '苹果',price: 100,num: 10,category: "水果"}, 
        {name: '香蕉',price: 15,num: 10,category: "水果"}, 
        {name: '雪梨',price: 65,num: 10,category: "水果"}, 
        {name: '宝马',price: 2500,num: 10,category: "汽车"},
        {name: '奔驰',price: 10025,num: 10,category: "汽车"}, 
        {name: '柑橘',price: 15,num: 10,category: "水果"}, 
        {name: '奥迪',price: 25,num: 10,category: "汽车"}
      ]
    }
  },
  filters: { // 局部过滤器
    currency(val) {
      return "$"+val
    },
    discount(val){
      return val*0.5
    },
    kind(val) {
      if(val == "水果") {
        return "水果类"
      }else {
        return "非水果类"
      }
    } 
  }
}
</script>

<!-- 添加'scoped'属性主要是为了限制以下样式仅在当前页面生效 -->
<style scoped>

</style>

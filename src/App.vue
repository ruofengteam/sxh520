<template>
  <div id="app">
    
    <van-goods-action>
      <van-goods-action-icon icon="chat-o" >
        客服
      </van-goods-action-icon>
      <van-goods-action-icon icon="cart-o" >
        购物车
      </van-goods-action-icon>
      <van-goods-action-button type="warning">
        加入购物车
      </van-goods-action-button>
      <van-goods-action-button type="danger" >
        立即购买
      </van-goods-action-button>
    </van-goods-action>
    <van-cell-group>
  <van-cell title="单元格" value="内容" />
  <van-cell title="单元格" value="内容" label="描述信息" />
</van-cell-group>
  </div>
</template>

<script>
import { GoodsAction,
  GoodsActionIcon,
  GoodsActionButton ,
  Cell, CellGroup} from 'vant';
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
     [GoodsAction.name]: GoodsAction,
    [GoodsActionIcon.name]: GoodsActionIcon,
    [GoodsActionButton.name]: GoodsActionButton,
    [CellGroup.name]: CellGroup,
    [Cell.name]: Cell
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

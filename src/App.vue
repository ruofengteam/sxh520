<template>
  <div id="app">
    <van-row type="flex" justify="space-around">
      <van-col span="6">
        <van-image
          round
          width="4.5rem"
          height="4.5rem"
          src="https://img01.yzcdn.cn/vant/cat.jpeg"
        />
      </van-col>
      <van-col span="6">span: 6</van-col>
      <van-col span="6">span: 6</van-col>
    </van-row>
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
  import { Col, Row } from 'vant';
  import { Image as VanImage } from 'vant';


export default {
  name: 'App',
  components: {
    [GoodsAction.name]: GoodsAction,
    [GoodsActionIcon.name]: GoodsActionIcon,
    [GoodsActionButton.name]: GoodsActionButton,
    [CellGroup.name]: CellGroup,
    [Cell.name]: Cell,
    [Col.name]: Col,
    [Row.name]: Row,
    [VanImage.name]: VanImage
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
  margin-top: 1rem;
}
body {
  font-size: 16px;
  background-color: #f8f8f8;
  -webkit-font-smoothing: antialiased;
}
</style>

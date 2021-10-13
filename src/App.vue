<template>
  <div id="app">
    
    <van-row class="row">
  <van-col span="3.2">
    <van-image
      round
      width="5.2rem"
      height="5.2rem"
      src="https://img.yzcdn.cn/vant/cat.jpeg"
    />
  </van-col>
  <van-col span="10" >
      <div class="up">姓名:某某</div>
      <div class="down"><van-tag type="primary" size="large">标签</van-tag></div>
  </van-col>
  <van-col span="8">span: 8</van-col>
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
  Cell, CellGroup,Tag, Button} from 'vant';
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
    [VanImage.name]: VanImage,
    [Tag.name]: Tag,
    [Button.name]: Button,
    
  },
  data () {
    return {
      
    }
  },
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
.row{
  height: 5.2rem;
}
.up {
 width: 8rem;
 height: 3rem;
 font-size: 1.2rem;
 text-align: left;
}
.down {
  width: 8rem;
  height: 2rem;
  position: absolute;
   text-align: left;
}
</style>

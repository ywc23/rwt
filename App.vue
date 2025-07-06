<style lang="scss">
@import "@/uni_modules/uview-ui/index.scss";
</style>

<script>
	export default {
		onLaunch: function() {
			console.log('App Launch')
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		}
	}
</script>

<style>
@import url("/static/iconfont/iconfont.css");
@import url("@/static/weui.min.css");

uni-modal {
  z-index: 999999 !important;
}
page {
	background-color: #f6f7fb;
  margin: 0 auto;
}
.container {
  width: 700rpx;
  margin: 0 auto;
}

.none {
	display: none;
}

.luck-text-color {
  color: #40A9FF;
}
.luck-text-default {
  color: #40A9FF;
}
.luck-text-danger {
	color: #FF0000;
}
.luck-text-price {
  color: #FF0000;
}
.uloadmore {
	margin: 30rpx 0;
}
button {
  padding: 0 !important;
}
.luck-btn {
  border-radius: 3px;
  text-align: center;
  padding: 5px 10px;
}
.luck-btn-default {
  background-color: #40A9FF;
  color: #fff;
}
.luck-btn-payment {
  background-color: #d8b66c;
  color: #fff;
}
.luck-btn-weixin {
  background-color: #1AAD19;
  color: #fff;
}
.luck-btn-secondary {
  background-color: #6c757d;
  color: #fff;
}
.luck-btn-danger {
  background-color: #FF0000;
  color: #fff;
}
//用来换颜色的
.luck-btn-wechaoya {
  background-color: #035bff;
  color: #fff;
}

/* form start */
.luck-form .weui-cell::before {
  right: 16px;
}
.weui-cell_select {
  padding: 32rpx !important;
}
.luck-form .items {
  background-color: #fff;
  overflow: hidden;
  font-size: 28rpx;
  border-radius: 3px;
}
.luck-form .items .top {
  padding: 32rpx;
}
.luck-form .items .top .stitle {
  font-weight: 400;
}
.luck-form .items .icon_question {
  margin-left: 3px;
}
.luck-form .items .span_required {
  color: #FF0000;
  margin-left: 3px;
}
.luck-form .items .span_remark {
  color: #999;
  margin-left: 3px;
  font-size: 24rpx;
}
.luck-form .custom_checkbox .box {
  width: 100%;
  margin-bottom: -10rpx;
  overflow: hidden;
}
.luck-form .custom_checkbox .box span {
  background-color: #eee;
  margin-right: 2%;
  float: left;
  margin-bottom: 10px;
  font-size: 28rpx;
  text-align: center;
  padding: 8px 12px;
  border-radius: 3px;
}
.luck-form .custom_checkbox .box span.on {
  background-color: #00B38A;
  color: #fff;
}
.luck-form .radio-group {
  margin-left: -10px;
  margin-bottom: -10px;
}
.luck-form .radio-group .radio {
  margin-left: 10px;
  margin-bottom: 10px;
  display: inline-block;
}
.luck-form .remind {
  display: flex;
  font-size: 24rpx;
  padding-left: 2px;
  color: #666;
}
.luck-form .remind .txt {
  margin-left: 2px;
  padding-top: 2px;
}
.luck-form .remind .link {
  color: #00B38A;
}
/* form end */

.luck-box {
  background-color: #fff;
  margin: 0 auto;
  padding: 30rpx 30rpx 30rpx 30rpx !important;
  border-radius: 3px;
  overflow: hidden;
}
.luck-box .stitle {
  padding-bottom: 30rpx;
}
.luck-box .stitle {
  font-weight: 600;
  letter-spacing: 2px;
  position: relative;
  padding-left: 26rpx;
  color: #666;
  font-size: 24rpx;
}
.luck-box .stitle::before {
  position: absolute;
  top: 8rpx;
  left: 0;
  width: 10rpx;
  height: 20rpx;
  border-radius: 32rpx;
  background: #40A9FF;
  content: '';
}

.result {
	text-align: center;
	padding: 60rpx;
}
.result .txt {}
.result .txt .iconfont {
	margin-right: 8rpx;
}
.result .des {
	margin-top: 20rpx;
	color: #999;
	font-size: 24rpx;
}
.result .btns {
	margin-top: 30rpx;
}
.result .btns .btn {
	margin-left: 10rpx;
}
.result .btns .btn:first-child {
	margin-left: 0;
}

/* payment start */
.payment {}
.payment .item {
	width: 100%;
	height: 120rpx;
	line-height: 120rpx;
	overflow: hidden;
	border-bottom: 1px solid #f5f5f5;
  font-size: 28rpx;
}
.payment .item .left {
	float: left;
}
.payment .item .icon {
	width: 54rpx;
  height: 54rpx;
  vertical-align: middle;
}
.payment .item .txt {
	margin-left: 5px;
}
.payment .item i {
	float: right;
}
.payment .item i:before {}
.payment .item.on i:before {
	color: #f4645f;
  content: '\e731';
}
.payment_foot {
  margin-top: 30rpx;
}
.payment_foot .description {
	color: #666;
	font-size: .875rem;
	margin-bottom: 30rpx;
}
.payment_foot .description .price_color {
	font-size: 40rpx;
  margin-right: 3px;
}
.payment_foot .pay_qrcode .msg {
	width: 150px;
	text-align: center;
	font-size: .875rem;
	letter-spacing: 3px;
}
.payment_foot .pay_qrcode .image {
	border: 1px solid #eee;
	width: 150px;
	height: 150px;
	line-height: 150px;
	text-align: center;
	margin-bottom: 5px;
	overflow: hidden;
}
.payment_foot .pay_qrcode .image img {
	max-width: 100%;
	max-height: 100%;
}
/* payment end */

/* 底部弹出支付 start */
.popup_payment {
  background-color: #ffffff;
  padding-bottom: 40rpx;
  border-top-left-radius: 8px;
  border-top-right-radius: 8px;
}
.popup_payment_container {
  width: 700rpx;
  margin: 0 auto;
}
.popup_payment_top {
  width: 100%;
  text-align: center;
  height: 90rpx;
  line-height: 90rpx;
  border-bottom: 1px solid #f5f5f5;
  overflow: hidden;
}
.popup_payment_top .close {
	position: absolute;
  top: 0;
	right: 40rpx;
	height: 90rpx;
	line-height: 90rpx !important;
	color: #999;
}
.popup_payment .items .item {
	width: 100%;
	height: 120rpx;
	line-height: 120rpx;
	overflow: hidden;
	border-bottom: 1px solid #f5f5f5;
  font-size: 28rpx;
}
.popup_payment .items .item .left {
	float: left;
}
.popup_payment .items .item .icon {
	width: 54rpx;
  height: 54rpx;
  vertical-align: middle;
}
.popup_payment .items .item .txt {
	margin-left: 5px;
}
.popup_payment .items .item i {
	float: right;
}
.popup_payment .items .item i:before {}
.popup_payment .items .item.on i:before {
	color: #f4645f;
  content: '\e731';
}
.popup_payment_foot {
  margin-top: 30rpx;
}
.popup_payment_foot .description {
	color: #666;
	font-size: .875rem;
	margin-bottom: 30rpx;
}
.popup_payment_foot .description .text-price {
	font-size: 20px;
  margin-right: 3px;
	color: #ff0000;
}
/* 底部弹出支付 end */
</style>
